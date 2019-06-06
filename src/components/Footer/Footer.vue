<template>
    <footer class="footer">
        <Contact/>
        <Info/>
    </footer>
</template>

<script>
import Contact from './Contact/Contact.vue'
import Info from './Info/Info.vue'

export default {
  name: 'Footer',
  components: {
      Contact,
      Info
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
