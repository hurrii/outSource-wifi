<template>
    <div class="container">
        <slot></slot>
    </div>
</template>

<script>

export default {
  name: 'Container.vue'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container {
    width: 100%;
    max-width: 280px;
    margin: 0 auto;
    overflow: hidden;

    @media screen and (min-width: 320px) {max-width: 87.5%;}
    @media screen and (min-width: 1440px) {max-width: 1160px;}
}
</style>
