<template>
  <div>
    <navigation/>

    <nuxt/>
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
    transition: all .1s ease-out;
    @apply inline-block my-6 py-4 px-6 bg-blue-600 border-blue-600 rounded-full text-white cursor-pointer;
  }

  .button:hover {
    transform: translateY(-1px);
    @apply bg-blue-800;
  }

  .button:active {
    transform: translateY(1px);
  }
</style>