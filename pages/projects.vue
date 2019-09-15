<template>
  <div class="container mx-auto py-32">
    <div class="project">
      <div class="project__image">
        <img class="w-full" src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300/v1565694490/jrtell/Opera_Snapshot_2019-09-15_174252_localhost">
      </div>
      <div class="project__content">
        <h2 class="project__title">JRTell.se</h2>
        <p>
          Latest version of my personal site. I rebuild it from scratch every now and then as I get new ideas and become bored of the current design.
          Built with Nuxt.js and tailwind.css.
          Statically generated with Nuxt and hosted with Netlify.
        </p>
      </div>
    </div>

    <div class="project">
      <div class="project__image">
        <img class="w-full" src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300/v1565695116/jrtell/nordland">
      </div>
      <div class="project__content">
        <h2 class="project__title">Nordland - Work In Progress</h2>
        <p>
          A personal browser-based online game I've been working on when I haven't felt like working on any other projects.<br>
          Built as a PWA (Progressive Web Application). Frontend is Nuxt.js with a Sailsjs backend.
        </p>
      </div>
    </div>

    <div class="project">
      <div class="project__image">
        <img class="w-full" src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300/v1552838252/jrtell/hemlagat">
      </div>
      <div class="project__content">
        <h2 class="project__title">Restaurang Hemlagat</h2>
        <p>
          My first jamstack!<br>
          The objective was to create a quick and simple website. I decided to use Nuxt.js and its
          static site generator, combined with Netlify for hosting and deployment.<br>
          The lunch menu needed to be dynamically updated by non-technical users. I settled for Contentful as the headless CMS and backend for this.
        </p>
        <a class="button" href="https://hemlagatjonkoping.se/" target="_blank" rel="noopener noreferrer">Check it out</a>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'projects'
  };
</script>

<style scoped>
  .project {
    @apply flex flex-col items-start mb-32;
  }

  .project__image {
    @apply rounded-lg overflow-hidden h-auto w-64 shadow-lg flex-shrink-0;
  }

  .project__title {
    @apply text-4xl;
  }

  .project__content {
    @apply px-6;
  }

  @screen sm {
    .project {
      @apply flex-row;
    }
  }
</style>
