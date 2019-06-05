<template>
  <div id="app">
    <Header/>
    <Content/>
    <Footer/>
  </div>
</template>

<script>
// eslint-disable-next-line
import sassStyles from './scss/import.scss'
import Header from './components/Header/Header.vue'
import Content from './components/Content/Content.vue'
import Footer from './components/Footer/Footer.vue'

export default {
  name: 'app',
  components: {
    Header,
    Content,
    Footer
  }
}
</script>

<style lang="scss">

#app {
  font-family: 'Graphik LCG', Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
