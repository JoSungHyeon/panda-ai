<template>
  <div class="mainPage">
    <Header />
  </div>
</template>

<script>
import Header from './components/Header.vue';

export default {
  components: {
    Header
  }
}
</script>

<style scoped>
.mainPage {
  background-color: #F2F2F2;
  width: 100vw;
  height: 100vh;
}
</style>
