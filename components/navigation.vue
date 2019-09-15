<template>
  <div class="navigation sticky top-0 overflow-x-auto z-10 -mb-24" :class="dynamicClasses">
    <nav class="container mx-auto flex items-center justify-between py-6 px-4">
      <div class="flex items-center flex-shrink-0 mr-6">
        <nuxt-link to="/" class="font-semibold text-2xl tracking-tight">John-Robin Tell</nuxt-link>
      </div>
      <div class="flex flex-grow items-center">
        <div class="flex-grow flex justify-end">
          <nuxt-link to="/projects" class="block px-4 py-2 whitespace-no-wrap">
            Projects
          </nuxt-link>
          <nuxt-link to="/work-history" class="block px-4 py-2 whitespace-no-wrap">
            Work history
          </nuxt-link>
          <nuxt-link to="/proficiencies" class="block px-4 py-2 whitespace-no-wrap">
            Proficiencies
          </nuxt-link>
          <nuxt-link to="/contact" class="block px-4 py-2 whitespace-no-wrap">Contact me</nuxt-link>
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

        return this.hasScrolled ? 'bg-white text-black shadow-lg' : 'text-white';
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
      console.log(this.$route);

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
</style>