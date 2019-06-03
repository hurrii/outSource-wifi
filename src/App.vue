<template>
  <div id="app">
    <Header/>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import sassStyles from './scss/import.scss'
import Header from './components/Header/Header.vue'
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    Header,
    HelloWorld
  }
}
</script>

<style lang="scss">

#app {
  font-family: 'SuisseIntl', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background: $paper;
}
</style>
