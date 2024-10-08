<template>
  <div class="bg-gray-500 text-gray-100 text-center pb-2">
    <div class="w-full background-banner">
      
      <h3 class="text-4xl uppercase mb-4 font-mono text-white-400 pt-12">Let's get this right for Linz in 2024</h3>

      <h2 class="text-5xl uppercase mb-4 font-mono pt-30">PostCity x IT-U (postuni)</h2>

    </div>

    <div class="max-w-3xl w-full mx-auto px-8 pt-10">
    <div class="pb-64 text-center">
      <!--<NuxtLink v-for="page in pages" :key="page" :to="page" class="underline mx-4">
        <span class="main-link" v-if="page == '/'">PostCity</span>
        <span class="secondary-link" v-else>+ {{ page }}</span>
      </NuxtLink>-->

      <h3 class="text-4xl uppercase mb-4 font-mono text-white-400 pt-12">What is this about and why now?</h3>

      <h5 class="text-md text-white-400">Now that the city <a href="https://www.nachrichten.at/politik/landespolitik/stadt-linz-zieht-bei-der-umwidmung-fuer-die-itu-die-notbremse;art383,3989606?utm_source=browser&utm_medium=push-notification&utm_campaign=cleverpush-1728293690">has backtracked</a>, rightfully, on the planned Dornach "Grüngürtel" extension, here is another chance for the PostCity location.</h5>

      <h4 class="text-md text-gray-400">Don't put short-term, boring business-as-usual before a truly transformative project opportunity, with, yes, business value as well, dear <b>Österreichische Post</b>* -</h4>

      <h4 class="text-md text-gray-400">*Current Owner of PostCity</h4>

      <h4 class="text-md text-gray-400">If Linz wants to continue to be a creative hub, it's <b>time to put the money where the mouth is</b>. </h4>
      
      <h4 class="text-md text-gray-400">This requires making yourself heard by city and government officials as well as private businesspeople owning the property in question.</h4>

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

      <h3 class="text-4xl uppercase mb-4 font-mono text-white-400 pt-12">Call to Action</h3>

      

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
</style>