<template>
  <div class="container mx-auto pt-32">
    <div class="employment">
      <h4 class="flex-1">Alektum Group</h4>
      <div class="flex-1">2019 - Current</div>
      <div class="flex-1">Front-End Developer</div>
      <div class="w-48">
        <a class="button my-0 py-2" href="https://www.alektumgroup.se/" target="_blank" rel="noopener noreferrer">Check it out</a>
      </div>
    </div>

    <div class="employment">
      <h4 class="flex-1">Rebel Walls</h4>
      <div class="flex-1">2016 - 2019</div>
      <div class="flex-1">Systems Developer</div>
      <div class="w-48">
        <a class="button my-0 py-2" href="https://rebelwalls.com/" target="_blank" rel="noopener noreferrer">Check it out</a>
      </div>
    </div>

    <div class="employment">
      <h4 class="flex-1">Self-employed</h4>
      <div class="flex-1">2013 - 2016</div>
      <div class="flex-1">Fullstack Developer</div>
      <div class="w-48"></div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'work-history'
  };
</script>

<style scoped>
  .employment {
    transition: all 200ms ease-in-out;

    @apply p-4 my-4 bg-gray-200 flex justify-between;
  }

  @media screen and (max-width: 600px) {
    .employment {
      @apply block;
    }

    .button {
      @apply mt-6;
    }
  }

  .employment:hover {
    @apply shadow-lg;
  }
</style>