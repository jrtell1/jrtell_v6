<template>
  <div>
    <div>
      <div class="container mx-auto sm:pt-48 pb-64 flex justify-center">
        <div class="p-4 w-full max-w-5xl relative">
          <div class="z-10 w-full max-w-md">
            <h1 class="text-3xl sm:text-5xl font-bold text-indigo-600" data-aos="fade-right" data-aos-delay="50">
              John-Robin Tell
            </h1>
            <h2 class="text-2xl sm:text-3xl" data-aos="fade-right" data-aos-delay="100">
              Fullstack Web Developer and freelancer based out of <span class="text-indigo-400">Borås</span>
            </h2>
            <div data-aos="fade-up" data-aos-delay="150">
              <a class="button" href="https://www.linkedin.com/in/john-robin-tell-b8bb235b/" target="_blank" rel="noopener noreferrer">Contact me on LinkedIn</a>
            </div>
          </div>

          <div class="opacity-75">
            <img class="illustration dev-illustration" data-aos="fade-left" src="/undraw_work_time_lhoj.svg" alt="illustration">
          </div>
        </div>
      </div>
    </div>

    <div class="container mx-auto py-24 lg:py-64 flex justify-between flex-col sm:flex-row relative">
      <div class="hidden lg:block opacity-75">
        <img class="illustration git-illustration" data-aos="fade-right" src="/undraw_coding_6mjf.svg" alt="illustration">
      </div>
      <div class="py-4 px-4 max-w-2xl z-10">
        <h2 class="second-subtitle text-4xl">I'm a developer with <span class="text-indigo-500">passion</span>!</h2>
        <p class="text-lg my-4">
          For as long as I can remember I've had an unending urge to create and build stuff!<br>
          I'm always working on improving myself, my character, my mind and my skills. I've always sought self-improvement,
          and the goal of becoming the best version of myself.
        </p>
        <p class="text-lg my-4">
          When I discovered code and development I knew I had found my calling. Now I write code and work on both my own projects and others every, single, day!
          I'm continually learning and creating. And I cannot imagine I'll ever stop!
        </p>
        <div data-aos="fade-up">
          <h3 class="my-4 text-xl font-semibold">Technologies I've worked with recently and absolutely love:</h3>
          <ul class="flex flex-wrap">
            <li class="p-2">JavaScript</li>
            <li class="p-2">VueJs</li>
            <li class="p-2">NuxtJs</li>
            <li class="p-2">TailwindCss</li>
            <li class="p-2">Typescript</li>
            <li class="p-2">Socket.io</li>
          </ul>
          <ul class="flex flex-wrap">
            <li class="p-2">Docker</li>
            <li class="p-2">Swoole</li>
            <li class="p-2">Laravel</li>
            <li class="p-2">Lumen</li>
            <li class="p-2">PHP</li>
            <li class="p-2">Redis</li>
            <li class="p-2">NodeJs</li>
          </ul>
        </div>
      </div>
    </div>

    <div class="container mx-auto pb-24 flex flex-col items-center">
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

    <div class="container mx-auto py-12 sm:pt-64 sm:pb-48 flex justify-between flex-col sm:flex-row relative">
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
        <p class="text-lg mt-4">
          I've built and worked on all kind of systems, like websites, blogs, professional administration systems and dashboards. I'm even building my own browser game!
          <br>If there's something you want done, send me a message and I'll get back to you.
        </p>

        <div data-aos="fade-up">
          <nuxt-link class="button" to="/projects">Check out some projects of mine</nuxt-link>
        </div>
      </div>
    </div>

<!--    <div class="container mx-auto sm:pb-32 pt-32 flex lg:items-center flex-col relative">-->
<!--      <h2 class="second-subtitle text-4xl px-4 lg:text-center">What can I do for <span class="text-indigo-500">you</span>?</h2>-->

<!--      <div class="sm:flex justify-around items-center my-8" data-aos="fade-up">-->
<!--        <div class="flex-1 p-4">-->
<!--          <img class="w-full shadow-md" src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_800/v1565694490/jrtell/Opera_Snapshot_2019-09-15_174252_localhost">-->
<!--        </div>-->
<!--        <div class="flex-1 px-4">-->
<!--          <h2 class="second-subtitle text-3xl">Websites</h2>-->
<!--          <p class="text-lg my-4">-->
<!--            I design and build websites, from the ground up. Simple ones like this one, and advanced ones with all kinds of features.-->
<!--          </p>-->
<!--        </div>-->
<!--      </div>-->

<!--      <div class="sm:flex sm:flex-row-reverse justify-around items-center my-8" data-aos="fade-up">-->
<!--        <div class="flex-1 p-4">-->
<!--          <img class="w-full shadow-md" src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_800/v1565694490/jrtell/Opera_Snapshot_2019-09-15_174252_localhost">-->
<!--        </div>-->
<!--        <div class="flex-1 px-4">-->
<!--          <h2 class="second-subtitle text-3xl">Administration systems</h2>-->
<!--          <p class="text-lg my-4">-->
<!--            I've worked on and built administration systems for multiple businesses. Both simpler ones and those who are fully tailored for the businesses need.-->
<!--          </p>-->
<!--        </div>-->
<!--      </div>-->

<!--      <div class="sm:flex justify-around items-center my-8" data-aos="fade-up">-->
<!--        <div class="flex-1 p-4">-->
<!--          <img class="w-full shadow-md" src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_800/v1565694490/jrtell/Opera_Snapshot_2019-09-15_174252_localhost">-->
<!--        </div>-->
<!--        <div class="flex-1 px-4">-->
<!--          <h2 class="second-subtitle text-3xl">Automations</h2>-->
<!--          <p class="text-lg my-4">-->
<!--            Do you have tedious tasks that you believe could be automated with software?-->
<!--          </p>-->
<!--        </div>-->
<!--      </div>-->
<!--    </div>-->

    <div class="container mx-auto pb-64 pt-48 flex lg:items-center flex-col relative">
      <h2 class="second-subtitle text-3xl px-4 lg:text-center">Send me a message<br>and lets chat</h2>
      <div class="px-4" data-aos="fade-up">
        <a class="button" href="https://www.linkedin.com/in/john-robin-tell-b8bb235b/" target="_blank" rel="noopener noreferrer">Contact me on LinkedIn</a>
      </div>
      <div class="px-4 text-xl mb-4" data-aos="fade-up">Or at</div>
      <div class="px-4 text-3xl" data-aos="fade-up">
        <span>john-robin@jrtell.se</span>
      </div>
      <div class="opacity-75">
        <img class="illustration contact-illustration" data-aos="fade-right" src="/undraw_envelope_n8lc.svg" alt="illustration">
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
  .illustration {
    @apply absolute z-0 pointer-events-none select-none;
  }

  .dev-illustration {
    height: 60rem;
    width: 60rem;
    left: 50px;
    top: -100px;
  }

  @screen sm {
    .dev-illustration {
      height: 60rem;
      width: 60rem;
      left: 450px;
      top: -300px;
    }
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
    top: 50px;
  }

  .contact-illustration {
    height: 30rem;
    width: 30rem;
    left: 200px;
    top: 290px;
  }

  @screen lg {
    .contact-illustration {
      height: 40rem;
      width: 40rem;
      left: 800px;
      top: 80px;
    }
  }

  .second-subtitle {
    font-weight: 300;
    word-spacing: 5px;
  }
</style>
