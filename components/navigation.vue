<template>
  <div class="navigation fixed top-0 inset-x-0 overflow-x-auto z-10" :class="dynamicClasses">
    <nav class="container mx-auto flex items-center justify-between py-4 px-4">
      <div class="hidden sm:flex items-center flex-shrink-0 mr-6">
        <nuxt-link to="/" class="link font-semibold text-2xl tracking-tight">John-Robin Tell</nuxt-link>
      </div>
      <div class="flex flex-grow items-center">
        <div class="flex-grow flex justify-end">
          <nuxt-link to="/" class="link link--home">Home</nuxt-link>
          <nuxt-link to="/projects" class="link">Projects</nuxt-link>
          <nuxt-link to="/work-history" class="link">Work history</nuxt-link>
          <nuxt-link to="/proficiencies" class="link">Proficiencies</nuxt-link>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
  export default {
    name: 'navigation',

    data() {
      return {
        hasScrolled: false
      }
    },

    computed: {
      dynamicClasses() {
        if (this.$route.path !== '/') {
          return 'bg-white text-black shadow-lg';
        }

        return this.hasScrolled ? 'bg-white text-gray-700 shadow-lg' : 'text-white';
      }
    },

    methods: {
      onScroll() {
        this.hasScrolled = window.scrollY > 0;
      }
    },

    created() {
      if (process.browser) {
        window.addEventListener('scroll', this.onScroll);
      }
    },

    mounted() {
      if (process.browser) {
        this.hasScrolled = window.scrollY > 0;
      }
    },

    destroyed() {
      window.removeEventListener('scroll', this.onScroll);
    }
  };
</script>

<style scoped>
  .navigation {
    transition: all .2s ease-out;
  }

  .link {
    @apply block px-4 py-2 whitespace-no-wrap;
  }

  @screen sm {
    .link--home {
      @apply hidden;
    }
  }

  .link::before,
  .link::after {
    @apply inline-block opacity-0;
    transition: transform 0.3s, opacity 0.2s;
  }

  .link:hover::before,
  .link:hover::after {
    @apply opacity-100;
    transform: translateX(0);
  }

  .link::before {
    margin-right: 10px;
    content: '{';
    transform: translateX(20px);
  }

  .link::after {
    margin-left: 10px;
    content: '}';
    transform: translateX(-20px);
  }

  .nuxt-link-exact-active::before {
    @apply opacity-100;
    margin-right: 10px;
    content: '{';
    transform: translateX(0);
  }

  .nuxt-link-exact-active::after {
    @apply opacity-100;
    margin-left: 10px;
    content: '}';
    transform: translateX(0);
  }
</style>