<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <HeaderPage/>
    <Main>
      <MainContent/>
      <MainMenu/>
    </Main>
    <Footer/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import HeaderPage from './components/HeaderPage.vue'
import MainContent from './components/MainContent.vue'
import MainMenu from './components/MainMenu.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    HeaderPage,
    MainContent,
    MainMenu,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
