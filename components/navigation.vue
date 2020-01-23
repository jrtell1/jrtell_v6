<template>
  <div class="fixed top-0 inset-x-0 overflow-x-auto z-50 bg-white text-gray-800 shadow">
    <nav class="container mx-auto flex items-center justify-between py-4 px-4">
      <div class="hidden sm:flex items-center flex-shrink-0 mr-6">
        <nuxt-link to="/" class="link font-semibold text-2xl tracking-tight">John-Robin Tell</nuxt-link>
      </div>
      <div class="flex flex-grow items-center">
        <div class="flex-grow flex sm:justify-end">
          <nuxt-link to="/" class="link link--home">Home</nuxt-link>
          <nuxt-link to="/projects" class="link">Projects</nuxt-link>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
  export default {
    name: 'navigation',
  };
</script>

<style scoped>
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
