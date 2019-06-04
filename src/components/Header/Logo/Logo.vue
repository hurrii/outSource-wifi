<template>
    <div class="header__logo logo">
        <span class="logo__part">outSource</span>
        <span class="logo__part logo__part_colored">/wi-fi</span>
    </div>
</template>

<script>
export default {
  name: 'Logo'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.logo {

    &__part {
        font-size: 20px;
        font-weight: bold;

        @media screen and (min-width: 600px) {font-size: 22px;}

        &_colored {
            color: $pink;
        }
    }
    
}
</style>
