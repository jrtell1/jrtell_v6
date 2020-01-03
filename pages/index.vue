<template>
  <div>
    <div>
      <div class="container mx-auto pt-48 pb-64 flex justify-center">
        <div class="p-4 w-full max-w-5xl">
          <div>
            <div class="z-10 w-full max-w-md">
              <h1 class="text-3xl sm:text-5xl font-bold text-indigo-600" data-aos="fade-right" data-aos-delay="50">
                John-Robin Tell
              </h1>
              <h2 class="text-2xl sm:text-3xl" data-aos="fade-right" data-aos-delay="100">
                Fullstack Web Developer and consultant based out of <span class="text-indigo-400">Borås</span>
              </h2>
              <div data-aos="fade-up" data-aos-delay="150">
                <a class="button" href="https://www.linkedin.com/in/john-robin-tell-b8bb235b/" target="_blank" rel="noopener noreferrer">Contact me on LinkedIn</a>
              </div>
            </div>
          </div>

          <div class="hidden lg:block opacity-75">
            <img class="illustration dev-illustration" data-aos="fade-left" src="/undraw_work_time_lhoj.svg" alt="illustration">
          </div>
        </div>
      </div>

<!--      <div class="illustrations hidden lg:block">-->
<!--        <img class="illustrations__dev" data-aos="fade-left" src="/undraw_work_time_lhoj.svg" alt="illustration">-->
<!--      </div>-->
    </div>

    <div class="container mx-auto py-64 flex justify-between flex-col sm:flex-row relative">
      <div class="hidden lg:block opacity-75">
        <img class="illustration hire-illustration" data-aos="fade-right" src="/undraw_version_control_9bpv.svg" alt="illustration">
      </div>

      <div class="max-w-3xl p-4 z-10">
        <h2 class="second-subtitle text-4xl">
          Hire me for projects and consulting
        </h2>
        <p class="text-lg">I'm a quick learner with a mind for producing and delivering results.</p>
        <p class="text-lg"></p>

        <div data-aos="fade-up" data-aos-delay="150">
          <nuxt-link class="button" to="/projects">Check out some projects of mine</nuxt-link>
        </div>
      </div>
    </div>

    <div class="container mx-auto py-32 text-center flex justify-around items-center flex-col sm:flex-row">
      <div class="max-w-2xl p-4">
        <h2 class="second-subtitle text-3xl">
          I create and design fully-featured web applications.
        </h2>
        <p class="text-lg">I build fast loading and reliable websites and web applications, with design and security in mind.</p>
        <p class="text-lg">I utilize modern frameworks and best practices, while still creating a unique design and tailored solution. For an awesome result.</p>

        <div class="flex items-center justify-center" data-aos="fade-up" data-aos-delay="150">
          <nuxt-link class="button" to="/projects">Check out my latest projects</nuxt-link>
        </div>
      </div>

      <div class="w-64 h-64 flex-shrink-0">
        <img data-aos="fade-left" src="/undraw_laravel_and_vue_59tp.svg" alt="illustration">
      </div>
    </div>

    <div class="bg-gray-800 py-48 skewed">
      <div class="container mx-auto text-center flex justify-around items-center flex-col sm:flex-row">
        <div class="w-64 h-64 flex-shrink-0">
          <img data-aos="fade-down-right" src="/undraw_developer_activity_bv83.svg" alt="illustration">
        </div>
        <div class="py-4 px-4 max-w-2xl text-gray-300">
          <h2 class="second-subtitle text-4xl text-gray-200">I'm a developer with passion.</h2>
          <p class="text-lg">
            I'm always working on something. I'm either rebuilding my personal portfolio website or working on some other side project.
          </p>
          <p class="text-lg">Always pushing to use the latest, but still mature, technologies.</p>
          <div data-aos="fade-up" data-aos-delay="150">
            <nuxt-link to="/proficiencies" class="button">Check out my skills</nuxt-link>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'index',
  }
</script>

<style scoped>
  /*.illustrations {*/
  /*  @apply absolute inset-0 overflow-hidden;*/
  /*}*/

  /*.illustrations__dev {*/
  /*  height: 60rem;*/
  /*  width: 60rem;*/
  /*  right: -250px;*/
  /*  opacity: 0.5;*/

  /*  @apply absolute z-0 pointer-events-none;*/
  /*}*/

  .illustration {
    @apply absolute z-0 pointer-events-none select-none;
  }

  .dev-illustration {
    height: 60rem;
    width: 60rem;
    right: -250px;
    top: 0;
  }

  .hire-illustration {
    height: 40rem;
    width: 40rem;
    left: -100px;
    top: 0;
  }

  .skewed {
    clip-path: polygon(0 0, 100% 20%, 100% 100%, 0 80%);
  }

  .second-subtitle {
    font-weight: 300;
    word-spacing: 5px;
  }
</style>
