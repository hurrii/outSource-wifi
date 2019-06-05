<template>
  <div id="app">
    <Header/>
    <Content/>
  </div>
</template>

<script>
// eslint-disable-next-line
import sassStyles from './scss/import.scss'
import Header from './components/Header/Header.vue'
import Content from './components/Content/Content.vue'

export default {
  name: 'app',
  components: {
    Header,
    Content
  }
}
</script>

<style lang="scss">

#app {
  font-family: 'Roboto', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
