<template>
  <div>
    <div>
      <div class="container mx-auto sm:pt-48 sm:pb-64 flex justify-center">
        <div class="p-4 w-full max-w-5xl relative">
          <img class="w-full mx-auto block mb-8 sm:hidden" data-aos="fade-left" src="/undraw_work_time_lhoj.svg" alt="illustration">

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

          <div class="hidden sm:block opacity-75">
            <img class="illustration dev-illustration" data-aos="fade-left" src="/undraw_work_time_lhoj.svg" alt="illustration">
          </div>
        </div>
      </div>

<!--      <div class="illustrations hidden lg:block">-->
<!--        <img class="illustrations__dev" data-aos="fade-left" src="/undraw_work_time_lhoj.svg" alt="illustration">-->
<!--      </div>-->
    </div>

    <div class="container mx-auto py-24 sm:py-64 flex justify-between flex-col sm:flex-row relative">
      <div class="hidden lg:block opacity-75">
        <img class="illustration hire-illustration" data-aos="fade-right" src="/undraw_version_control_9bpv.svg" alt="illustration">
      </div>

      <div class="max-w-3xl p-4 z-10">
        <h2 class="second-subtitle text-4xl">
          Hire me for <span class="text-indigo-500">projects</span> and <span class="text-indigo-500">consulting</span>
        </h2>
        <p class="text-lg my-4">
          I'm an incredibly driven and quick learner with a mind for producing and delivering real results!
        </p>
        <p class="text-lg my-4">
          I've built and worked on all kind of systems, like websites, blogs, professional administrationsystems and dashboards. I'm even building my own browser game!
          <br>If there's something you want done, send me a message, I can most likely do it.
        </p>

        <div data-aos="fade-up">
          <nuxt-link class="button" to="/projects">Check out some projects of mine</nuxt-link>
        </div>
      </div>
    </div>

    <div class="container mx-auto sm:pb-64 flex flex-col items-center">
      <div class="px-4">
        <h2 class="second-subtitle text-4xl">
          Some of my <span class="text-indigo-500">clients</span>
        </h2>
        <div class="sm:flex justify-around my-8 shadow-lg rounded-lg" data-aos="fade-up">
          <img class="w-48 p-4" src="/Rebel_Walls_Logo_tag.svg" alt="illustration">
          <div class="px-4">
            <h3 class="text-2xl font-semibold mt-4">Rebel Walls</h3>
            <p>A high-quality premium wall murals producing business with customers all around the globe.</p>
            <a class="button" href="https://rebelwalls.com/" target="_blank" rel="noopener noreferrer">Check them out</a>
          </div>
        </div>
      </div>
    </div>

    <div class="bg-gray-100 py-64 skewed">
      <div class="container mx-auto flex justify-between flex-col sm:flex-row relative">
        <div class="hidden lg:block opacity-75">
          <img class="illustration git-illustration" data-aos="fade-right" src="/undraw_coding_6mjf.svg" alt="illustration">
        </div>
        <div class="py-4 px-4 max-w-2xl z-10">
          <h2 class="second-subtitle text-4xl">I'm a developer with <span class="text-indigo-500">passion</span></h2>
          <p class="text-lg my-4">
            I'm always working on something. I'm either rebuilding my personal portfolio website or working on some other side project.
          </p>
          <p class="text-lg mt-4">Always pushing to use the latest, but still mature, technologies.</p>
          <div data-aos="fade-up">
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
    left: 450px;
    top: -300px;
  }

  .hire-illustration {
    height: 40rem;
    width: 40rem;
    right: 800px;
    top: 50px;
  }

  .git-illustration {
    height: 40rem;
    width: 40rem;
    right: 700px;
    top: -200px;
  }

  .skewed {
    clip-path: polygon(0 0, 100% 20%, 100% 100%, 0 80%);
  }

  .second-subtitle {
    font-weight: 300;
    word-spacing: 5px;
  }
</style>
