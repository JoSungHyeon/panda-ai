<template>
  <!-- <Development /> -->
  <Header />
  <Intro />
  <About />
</template>

<script>
import Header from './components/Header.vue';
import Development from './components/Development.vue';
import Intro from './components/Intro.vue';
import About from './components/About.vue';

import Lenis from 'lenis'

export default {
  name: 'App',

  components: {
    Header,
    Development,
    Intro,
    About
  },

  data() {
    return {
      lenis: null
    }
  },

  mounted() {
    this.lenis = new Lenis({
      duration: 1.2,
      smoothWheel: true
    })

    const raf = (time) => {
      this.lenis.raf(time)
      requestAnimationFrame(raf)
    }

    requestAnimationFrame(raf)
  },

  beforeUnmount() {
    this.lenis?.destroy()
  },

  methods() {
    this.lenis = new Lenis({
      duration: 1.2,
      smoothWheel: true,
      wheelMultiplier: 1,
      touchMultiplier: 1
    })
  }
}
</script>

<style scoped>

</style>