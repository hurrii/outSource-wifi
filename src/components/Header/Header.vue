<template>
  <header class="header header_shadow">
      <Logo/>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolorum reiciendis soluta labore, illum cumque dolor doloribus veniam aliquid officiis. Ut doloribus dolore cum velit laborum rem odit! Tempora, commodi animi.</p>
  </header>
</template>

<script>
import Logo from './Logo/Logo.vue'

export default {
  name: 'Header',
  components: {
    Logo
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .header {
        color: $black;
        background: $white;

        &_shadow {
          box-shadow: 0 5px 15px 0 rgba(0, 0, 0, 0.1);
        }
    }

</style>
