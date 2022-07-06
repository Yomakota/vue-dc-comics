<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <HeaderPage/>
    <Main>
      <MainContent/>
      <MainMenu/>
    </Main>
    <Footer>
      <FooterLinks/>
    </Footer>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import HeaderPage from './components/HeaderPage.vue'
import MainContent from './components/MainContent.vue'
import MainMenu from './components/MainMenu.vue'
import FooterLinks from './components/FooterLinks.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    HeaderPage,
    MainContent,
    MainMenu,
    FooterLinks,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
