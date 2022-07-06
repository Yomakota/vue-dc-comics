<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <HeaderPage/>
    <main>
      <MainContent/>
      <MainMenu/>
    </main>
    <footer>
      <FooterLinks/>
      <FooterBottom/>
    </footer>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import HeaderPage from './components/HeaderPage.vue'
import MainContent from './components/MainContent.vue'
import MainMenu from './components/MainMenu.vue'
import FooterLinks from './components/FooterLinks.vue'
import FooterBottom from './components/FooterBottom.vue'


export default {
  name: 'App',
  components: {
    // HelloWorld
    HeaderPage,
    MainContent,
    MainMenu,
    FooterLinks,
    FooterBottom
  }
}
</script>

<style lang="scss">
@import "./assets/style/commons.scss";
</style>
