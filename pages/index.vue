<template>
  <div>
    <div class="hero bg-cover bg-bottom text-white">
      <div class="container mx-auto pt-48 pb-24 flex">
        <div class="p-4 lg:w-3/5 flex flex-col sm:flex-row items-center sm:items-start">
          <img class="rounded-full mr-4 shadow-lg border-4 h-32 w-32 pointer-events-none" src="https://media.licdn.com/dms/image/C4D03AQEB3J6LLFWEmg/profile-displayphoto-shrink_200_200/0?e=1574294400&v=beta&t=XXHS801SgSqyb2b-9JlUOwsUJyh50cSgbR0WEGo-t0s" alt="portrait">
          <div>
            <h1 class="text-5xl font-bold">John-Robin Tell</h1>
            <h2 class="text-4xl">Fullstack Developer</h2>
          </div>
        </div>
      </div>
      <div>
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
          <path fill="#fff" fill-opacity="1" d="M0,160L80,149.3C160,139,320,117,480,122.7C640,128,800,160,960,160C1120,160,1280,128,1360,112L1440,96L1440,320L1360,320C1280,320,1120,320,960,320C800,320,640,320,480,320C320,320,160,320,80,320L0,320Z"></path>
        </svg>
      </div>
    </div>

    <div class="container mx-auto py-32 text-center flex justify-around items-center flex-col sm:flex-row">
      <div class="flex flex-col justify-center max-w-2xl">
        <h2 class="second-subtitle text-3xl px-4">
          I build websites and fully-featured web applications.
        </h2>
        <p class="text-lg">I build fast loading and reliable websites and web applications, with design and security in mind.</p>
        <p class="text-lg">I utilize modern frameworks and best practices, while still creating a unique design and tailored solution. For an awesome result.</p>

        <div class="flex items-center justify-center">
          <nuxt-link class="inline-block my-6 py-4 px-6 bg-blue-600 border-blue-600 rounded-full text-white" to="/projects">Check out my latest projects</nuxt-link>
        </div>
      </div>

      <div class="w-64 h-64 flex-shrink-0">
        <img src="/undraw_laravel_and_vue_59tp.svg" alt="Programmer illustration">
      </div>
    </div>

    <div class="bg-gray-100 py-48 skewed">
      <div class="container mx-auto text-center flex justify-around items-center flex-col sm:flex-row">
        <div class="w-64 h-64 flex-shrink-0">
          <img src="/undraw_developer_activity_bv83.svg" alt="Programmer illustration">
        </div>
        <div class="py-4 px-4 flex flex-col items-center max-w-2xl">
          <h2 class="second-subtitle text-4xl">I'm a developer with passion.</h2>
          <p class="text-xl">
            I'm always working on something. I'm either rebuilding my personal portfolio website or working on some other side project.
          </p>
          <a class="inline-block my-6 py-4 px-6 bg-blue-600 border-blue-600 rounded-full text-white">Check out my skills</a>
        </div>
      </div>
    </div>

    <div class="py-48">
      <div class="container mx-auto text-center flex justify-around items-center flex-col sm:flex-row">
        <div class="py-4 px-4 flex flex-col items-center max-w-2xl">
          <h2 class="second-subtitle text-4xl">Current occupation.</h2>
          <p class="text-xl">Employed full-time and freelancing on the side.</p>
          <a class="inline-block my-6 py-4 px-6 bg-blue-600 border-blue-600 rounded-full text-white" href="https://www.linkedin.com/in/john-robin-tell-b8bb235b/" target="_blank" rel="noopener noreferrer">Contact me on LinkedIn</a>
        </div>
        <div class="w-64 h-64 flex-shrink-0">
          <img src="/undraw_work_time_lhoj.svg" alt="Programmer illustration">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {

  }
</script>

<style scoped>
  .hero {
    background-image: linear-gradient(
      rgba(20,20,20, .32),
      rgba(20,20,20, .7)),
      url('https://images.unsplash.com/photo-1552661014-41c6afdfb259?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2100&q=100');
  }

  .skewed {
    clip-path: polygon(0 0, 100% 20%, 100% 100%, 0 80%);
  }

  .second-subtitle {
    font-weight: 300;
    color: #526488;
    word-spacing: 5px;
  }
</style>