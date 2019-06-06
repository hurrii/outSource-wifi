<template>
    <div class="logo">
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
    width: 203px;
    flex: 1;
    white-space: nowrap;
    padding: 20px 20px 20px 0;

    &__part {
        font-size: 26px;
        font-weight: bold;

        @media screen and (min-width: 768px) {font-size: 22px;}

        &_colored {
            color: $pink;
        }
    }
    
}
</style>
