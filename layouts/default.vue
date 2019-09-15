<template>
  <div>
    <div class="sticky top-0 bg-white overflow-x-auto shadow-lg z-10">
      <nav class="container mx-auto flex items-center justify-between text-black py-6 px-4">
        <div class="flex items-center flex-shrink-0 mr-6">
          <nuxt-link to="/" class="font-semibold text-2xl tracking-tight">John-Robin Tell</nuxt-link>
        </div>
        <div class="flex flex-grow items-center">
          <div class="flex text-md -mx-4">
            <a href="#responsive-header" class="block px-4 whitespace-no-wrap">
              Projects
            </a>
            <a href="#responsive-header" class="block px-4 whitespace-no-wrap">
              Work history
            </a>
            <a href="#responsive-header" class="block px-4 whitespace-no-wrap">
              Proficiencies
            </a>
          </div>
          <div class="flex-grow flex justify-end">
            <a href="#" class="inline-block px-4 py-2 whitespace-no-wrap">Contact me</a>
          </div>
        </div>
      </nav>
    </div>

    <nuxt />
  </div>
</template>

<style>
  body {
    font-family: 'Montserrat', sans-serif;
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