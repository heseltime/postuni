<template>
  <div class="bg-gray-500 text-gray-100 text-center pb-2">
    <div class="w-full background-banner">
      
      <h3 class="text-4xl uppercase mb-4 font-mono text-white-400 pt-12">Let's get this right for Linz in 2024</h3>

      <h2 class="text-5xl uppercase mb-4 font-mono pt-30">PostCity x IT-U (postuni)</h2>

      <h3 class="text-4xl uppercase mb-4 font-mono text-red-400 pt-12">While the initial drive came top-down from politics, Linz is shaping the project to make it actually work for the city.</h3>

      <div class="bg-gray-500 text-gray-100 text-center">
        <div class="w-full background-banner flashy-banner-text">
          
          <h3 class="text-4xl uppercase mb-4 font-mono pt-12">Time for Linz to be Heard!</h3>

          <h2 class="text-5xl uppercase mb-4 font-mono pt-30">Let's move the university to PostCity</h2>

        </div>
      </div>

    </div>

    <div class="max-w-3xl w-full mx-auto px-8 pt-10">
      <div class="highlight-text-intro pb-64 text-center">
        <h3 class="text-4xl uppercase mb-4 font-mono text-white-400 pt-12">What is this about and why now?</h3>
        <h5 class="text-md text-white-400">
          Now that the city <a href="https://www.nachrichten.at/politik/landespolitik/stadt-linz-zieht-bei-der-umwidmung-fuer-die-itu-die-notbremse;art383,3989606?utm_source=browser&utm_medium=push-notification&utm_campaign=cleverpush-1728293690" target="_blank">has backtracked</a> on the planned Dornach "Grüngürtel" extension, here is another chance for the PostCity location.
        </h5>
        <h3 class="text-md text-gray-300">Don't put short-term, boring business-as-usual before a truly transformative project opportunity, with, yes, business value as well, dear <b>Österreichische Post</b>* -</h3>
        <h4 class="text-md text-gray-300">* <b>Current Owner of PostCity</b></h4>
        <h3 class="text-md text-gray-300">If Linz wants to continue to be a creative hub, it's <b>time to put the money where the mouth is</b>.</h3>
        <h4 class="text-md text-gray-300">This requires making yourself heard by city and government officials as well as private businesspeople owning the property in question.</h4>
      </div>

    <Nuxt />

      <!--<div
        class="fixed left-0 w-full h-0 border-t-2 border-dashed border-black"
        :style="{ top: triggerTop + 'px' }"
      >
        <p>Offset: {{ offset }}</p>
      </div>-->

    <div class="pb-64 text-center">
      <!--<NuxtLink v-for="page in pages" :key="page" :to="page" class="underline mx-4">
        <span class="main-link" v-if="page == '/'">PostCity</span>
        <span class="secondary-link" v-else>+ {{ page }}</span>
      </NuxtLink>-->

      <h3 class="text-4xl uppercase mb-4 font-mono text-white-400 pt-12">Who We Are</h3>

      

    </div>

    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      pages: ['/', 'Basic', 'Progress', 'StickyGraphic1', 'StickyGraphic2'],
      triggerTop: 0,
      offset: 0.6
    }
  },
  mounted () {
    window.addEventListener('resize', this.handleResize)
    this.handleResize()
  },
  methods: {
    handleResize () {
      this.triggerTop = this.offset * window.innerHeight
    }
  }
}
</script>

<style scoped>
.main-link {
  font-size: 2em;
}

.secondary-link {
  color: #bbb;
  text-decoration: none;
}

.background-banner {
  background-image: url('@/assets/img/postuni.jpg');
  background-size: cover;
  background-position: center;
  height: 600px;
}

.highlight-text-intro {
  background-color: rgba(0, 0, 0, 0.6); /* Semi-transparent dark overlay */
  padding: 3em 2em; /* Extra padding for vertical spacing */
  border-radius: 8px;
  max-width: 800px;
  margin: 0 auto;
  color: #e0e6ed;
  text-align: left; /* Align text to the left */
}

.highlight-text-intro h3 {
  color: #ffffff;
  text-shadow: 1px 1px 4px rgba(0, 0, 0, 0.4);
  margin-bottom: 1.5em; /* Additional bottom margin for spacing */
}

.highlight-text-intro h4,
.highlight-text-intro h5 {
  font-weight: 300;
  color: #e0e6ed;
  margin-bottom: 1.2em; /* Additional spacing between elements */
}

.highlight-text-intro a {
  color: #00bcd4;
  font-weight: bold;
  text-decoration: underline;
  transition: color 0.3s ease;
}

.highlight-text-intro a:hover {
  color: #0097a7;
}

.highlight-text-intro b {
  font-weight: bold;
  color: #ffffff;
}

.flashy-banner-text {
  text-align: center;
  padding: 3em 1em;
  background: linear-gradient(135deg, #ff6b6b, #ffd93d, #1dd3b0, #0078d7); /* Gradient background */
  background-size: 300% 300%;
  animation: gradientAnimation 8s ease infinite; /* Gradient animation */
}

.flashy-banner-text h3, .flashy-banner-text h2 {
  color: #ffffff;
  font-weight: bold;
  text-transform: uppercase;
  text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.4); /* Shadow for depth */
}

.flashy-banner-text h3 {
  font-size: 3rem;
  margin-bottom: 0.5em;
}

.flashy-banner-text h2 {
  font-size: 4.5rem;
  font-weight: 900;
  margin-bottom: 1em;
}

/* Gradient animation */
@keyframes gradientAnimation {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}


</style>