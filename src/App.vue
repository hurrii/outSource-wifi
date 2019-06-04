<template>
  <div id="app">
    <Header/>
  </div>
</template>

<script>
// eslint-disable-next-line
import sassStyles from './scss/import.scss'
import Header from './components/Header/Header.vue'
// import HelloWorld from './components/HelloWorld.vue'
// eslint-disable-next-line
import Container from './components/Container.vue'

export default {
  name: 'app',
  components: {
    Header
  }
}
</script>

<style lang="scss">

#app {
//@import url('./scss/layout/layout.scss');

  font-family: 'SuisseIntl', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;


}
</style>
