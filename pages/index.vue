<template>
  <div>
    <div class="hero bg-cover bg-center text-white">
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
<!--        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#fff" fill-opacity="1" d="M0,224L34.3,213.3C68.6,203,137,181,206,160C274.3,139,343,117,411,128C480,139,549,181,617,181.3C685.7,181,754,139,823,101.3C891.4,64,960,32,1029,21.3C1097.1,11,1166,21,1234,21.3C1302.9,21,1371,11,1406,5.3L1440,0L1440,320L1405.7,320C1371.4,320,1303,320,1234,320C1165.7,320,1097,320,1029,320C960,320,891,320,823,320C754.3,320,686,320,617,320C548.6,320,480,320,411,320C342.9,320,274,320,206,320C137.1,320,69,320,34,320L0,320Z"></path></svg>-->
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#fff" fill-opacity="1" d="M0,224L48,213.3C96,203,192,181,288,181.3C384,181,480,203,576,213.3C672,224,768,224,864,208C960,192,1056,160,1152,133.3C1248,107,1344,85,1392,74.7L1440,64L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path></svg>
      </div>
    </div>

    <div class="container mx-auto py-32 text-center flex justify-around items-center flex-col sm:flex-row">
      <div class="flex flex-col justify-center max-w-2xl p-4">
        <h2 class="second-subtitle text-3xl">
          I create and design fully-featured web applications.
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

    <div class="bg-gray-800 py-48 skewed">
      <div class="container mx-auto text-center flex justify-around items-center flex-col sm:flex-row">
        <div class="w-64 h-64 flex-shrink-0">
          <img src="/undraw_developer_activity_bv83.svg" alt="Programmer illustration">
        </div>
        <div class="py-4 px-4 flex flex-col items-center max-w-2xl text-gray-300">
          <h2 class="second-subtitle text-4xl text-gray-200">I'm a developer with passion.</h2>
          <p class="text-lg">
            I'm always working on something. I'm either rebuilding my personal portfolio website or working on some other side project.
          </p>
          <p class="text-lg">Always pushing to use the latest, but still mature, technologies.</p>
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
      url('https://res.cloudinary.com/jrtell/image/upload/c_fill,e_blur:300,f_auto,h_800,q_auto,w_1920/v1568554332/jrtell/fabian-grohs-P2SkP_PXhlU-unsplash');
    background-repeat: no-repeat;
  }

  .skewed {
    clip-path: polygon(0 0, 100% 20%, 100% 100%, 0 80%);
  }

  .second-subtitle {
    font-weight: 300;
    word-spacing: 5px;
  }
</style>