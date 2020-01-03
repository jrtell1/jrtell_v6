<template>
  <div class="container mx-auto pt-20">
    <div class="mb-12 px-4">
      <h1 class="text-3xl sm:text-5xl font-bold text-indigo-600" data-aos="fade-right" data-aos-delay="50">
        Projects
      </h1>
      <h2 class="text-2xl sm:text-3xl" data-aos="fade-right" data-aos-delay="100">
        Below are my latest personal projects of note
      </h2>
    </div>

<!--    <div class="project">-->
<!--      <div class="project__image" data-aos="fade-right">-->
<!--        <img class="w-full" src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300/v1565694490/jrtell/Opera_Snapshot_2019-09-15_174252_localhost">-->
<!--      </div>-->
<!--      <div class="project__content">-->
<!--        <h2 class="project__title" data-aos="fade-up">JRTell.se</h2>-->
<!--        <p data-aos="fade-up" data-aos-delay="50">-->
<!--          Latest version of my personal site. I rebuild it from scratch every now and then as I get new ideas and become bored of the current design.-->
<!--          Built with Nuxt.js and tailwind.css.-->
<!--          Statically generated with Nuxt and hosted with Netlify.-->
<!--        </p>-->
<!--      </div>-->
<!--    </div>-->

    <div class="project">
      <div class="project__image" data-aos="fade-right">
        <img class="w-full" src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300/v1565695116/jrtell/nordland">
      </div>
      <div class="project__content">
        <h2 class="project__title" data-aos="fade-up">Skaldby - Work In Progress</h2>
        <p data-aos="fade-up" data-aos-delay="50">
          A personal browser-based online game I've been working on when I haven't felt like working on any other projects. Both for fun and for pushing my skills farther.<br>
          Built as a PWA (Progressive Web Application) on a microservice architecture.<br>
          Built around a central API powered by Lumen (PHP framework) with a NuxtJs frontend (VueJs and NodeJs) and a Redis service for caching.
          Also running one NodeJs service for processing fights and another NodeJs service for pushing notifications and real-time updates to the clients browser.<br>
          All containerized by Docker.
        </p>
        <a class="button" href="https://nordland.jrtell.se/" target="_blank" rel="noopener noreferrer" data-aos="fade-up" data-aos-delay="100">Check it out</a>
      </div>
    </div>

<!--    <div class="project">-->
<!--      <div class="project__image" data-aos="fade-right" data-aos-delay="150">-->
<!--        <img class="w-full" src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300/v1552838252/jrtell/hemlagat">-->
<!--      </div>-->
<!--      <div class="project__content">-->
<!--        <h2 class="project__title" data-aos="fade-up">Restaurang Hemlagat</h2>-->
<!--        <p data-aos="fade-up" data-aos-delay="50">-->
<!--          My first jamstack!<br>-->
<!--          The objective was to create a quick and simple website. I decided to use Nuxt.js and its-->
<!--          static site generator, combined with Netlify for hosting and deployment.<br>-->
<!--          The lunch menu needed to be dynamically updated by non-technical users. I settled for Contentful as the headless CMS and backend for this.-->
<!--        </p>-->
<!--        <a class="button" href="https://hemlagatjonkoping.se/" target="_blank" rel="noopener noreferrer" data-aos="fade-up" data-aos-delay="100">Check it out</a>-->
<!--      </div>-->
<!--    </div>-->
  </div>
</template>

<script>
  export default {
    name: 'projects'
  };
</script>

<style scoped>
  .project {
    @apply flex flex-col items-center mb-32;
  }

  .project__image {
    @apply rounded-lg overflow-hidden h-auto w-64 shadow-lg flex-shrink-0 mb-4;
  }

  .project__title {
    @apply text-4xl font-semibold;
  }

  .project__content {
    @apply px-6;
  }

  @screen sm {
    .project {
      @apply flex-row items-start;
    }
  }
</style>
