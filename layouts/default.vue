<template>
  <div>
    <navigation/>

    <div class="mt-24">
      <nuxt/>
    </div>
  </div>
</template>

<script>
  import Navigation from '../components/navigation';

  export default {
    components: { Navigation }
  };
</script>

<style>
  body {
    font-family: 'Montserrat', sans-serif;
    overflow-x: hidden;
  }

  html {
    overflow-x: hidden;
    overflow-y: scroll;
  }

  .page-enter-active {
    transition: opacity 0.125s ease-out;
  }

  .page-leave-active {
    transition: opacity 0.125s ease-in;
  }

  .page-enter,
  .page-leave-active {
    opacity: 0;
  }

  .button {
    transition: all .25s ease-out;
    @apply inline-block my-6 px-8 bg-indigo-500 rounded text-white cursor-pointer h-12 inline-flex items-center;
  }

  .button:hover,
  .button:focus {
    @apply bg-indigo-400;
  }

  .button:active {
    @apply bg-indigo-600;
  }
</style>
