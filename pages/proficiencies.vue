<template>
  <div class="container mx-auto pt-20">
    <div class="card mb-16">
      <div class="card__title">
        <h2 class="text-3xl mr-8" data-aos="fade-right">Front-End</h2>
      </div>
      <div class="card__content" data-aos="fade-up">
        <div class="proficiencies__column">
          <h4 class="proficiencies__title">Languages</h4>
          <ul class="proficiencies__list">
            <li>HTML</li>
            <li>CSS</li>
            <li>SCSS</li>
            <li>JavaScript</li>
            <li>Typescript</li>
          </ul>
        </div>
        <div class="proficiencies__column">
          <h4 class="proficiencies__title">Frameworks and libraries</h4>
          <ul class="proficiencies__list">
            <li>VueJs</li>
            <li>NuxtJs</li>
            <li>Socket.io</li>
            <li>Tailwind.css</li>
            <li>Bulma</li>
            <li>AnimeJs</li>
            <li>AOS</li>
          </ul>
        </div>
        <div class="proficiencies__column">
          <h4 class="proficiencies__title">Tools</h4>
          <ul class="proficiencies__list">
            <li>Webpack</li>
          </ul>
        </div>
      </div>
    </div>

    <div class="card my-16">
      <div class="card__title">
        <h2 class="text-3xl mr-8" data-aos="fade-right">Back-End</h2>
      </div>
      <div class="card__content" data-aos="fade-up">
        <div class="proficiencies__column">
          <h4 class="proficiencies__title">Languages</h4>
          <ul class="proficiencies__list">
            <li>PHP</li>
            <li>SQL</li>
            <li>NodeJs</li>
          </ul>
        </div>
        <div class="proficiencies__column">
          <h4 class="proficiencies__title">Frameworks and libraries</h4>
          <ul class="proficiencies__list">
            <li>Laravel/Lumen</li>
            <li>Socket.io</li>
            <li>SailsJs</li>
          </ul>
        </div>
        <div class="proficiencies__column">
          <h4 class="proficiencies__title">Tools</h4>
          <ul class="proficiencies__list">
            <li>Vagrant</li>
            <li>Composer</li>
          </ul>
        </div>
      </div>
    </div>

    <div class="card my-16">
      <div class="card__title">
        <h2 class="text-3xl mr-8" data-aos="fade-right">DevOps</h2>
      </div>
      <div class="card__content" data-aos="fade-up">
        <div class="proficiencies__column">
          <ul class="proficiencies__list">
            <li>Docker</li>
            <li>Netlify</li>
            <li>Git</li>
            <li>Nginx</li>
            <li>Ubuntu/Linux</li>
            <li>Cloudinary CDN</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'proficiencies'
  };
</script>

<style scoped>
  .card {
    @apply flex flex-col shadow overflow-hidden;
  }

  @screen sm {
    .card {
      @apply flex-row;
    }
  }

  .card__title {
    transition: all 200ms ease-out;
    @apply flex items-center justify-center p-16 text-black relative;
  }

  .card__title > * {
    @apply relative z-10;
  }

  .card__title::after {
    transition: all 100ms ease-out;
    content: '';
    clip-path: polygon(0 0, 0% 0%, 0% 100%, 0 100%);
    @apply block absolute inset-0 z-0 bg-indigo-500;
  }

  .card:hover .card__title {
    @apply text-white;
  }

  .card:hover .card__title::after {
    clip-path: polygon(0 0, 100% 0%, 80% 100%, 0 100%);
  }

  .card__content {
    @apply p-4;
  }

  .proficiencies__column {
    @apply flex-1;
  }

  .proficiencies__title {
    font-size: 18px;
  }

  .proficiencies__list {
    @apply flex p-0 flex-wrap;
  }

  .proficiencies__list li {
    list-style: none;
    padding: 2px 10px;

    @apply flex items-center;
  }

  .proficiencies__list li::before {
    border-radius: 3px;
    content: "";
    height: 10px;
    width: 10px;
    margin-right: 5px;

    @apply inline-block bg-indigo-500;
  }
</style>
