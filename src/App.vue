<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <HeaderPage />
    <JumbotronComic />
    <MainDcComics />
    <MainFooter />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import HeaderPage from './components/HeaderPage.vue';
import MainDcComics from './components/MainDcComics.vue'
import MainFooter from './components/MainFooter.vue';
import JumbotronComic from './components/JumbotronComic.vue';

export default {
  name: 'App',
  components: {
    // HelloWorld
    HeaderPage,
    MainDcComics,
    JumbotronComic,
    MainFooter,
  }
}
</script>

<style lang="scss">
@import "./assets/style/commons.scss";
</style>
