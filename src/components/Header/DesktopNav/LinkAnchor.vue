<template>
    <a href="#" class="linkAnchor" v-bind:class="anchorColor">{{ anchorText }}</a>
</template>

<script>
export default {
    name: 'LinkAnchor',
    props: {
        anchorText: String,
        anchorColor: String
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .anchor-black {
        color: $black;
    }
    .anchor-grey {
        color: $grey;
    }
</style>
