<template>
    <ul class="header__desktop-nav desktop-nav">
        <li>
            <linkAnchor v-bind:anchorText="anchorTextValue[0]" v-bind:anchorColor="anchorColorValue"/>
        </li>
        <li>
            <linkAnchor v-bind:anchorText="anchorTextValue[1]" v-bind:anchorColor="anchorColorValue"/>
        </li>
        <li>
            <linkAnchor v-bind:anchorText="anchorTextValue[2]" v-bind:anchorColor="anchorColorValue"/>
        </li>
        <li>
            <linkAnchor v-bind:anchorText="anchorTextValue[3]" v-bind:anchorColor="anchorColorValue"/>
        </li>
    </ul>
</template>

<script>
import linkAnchor from './LinkAnchor.vue'

export default {
    name: 'DesktopNav',
    components: {
        linkAnchor
    },
    data () {
        return {
            anchorTextValue: ["О компании", "Проекты", "Новости", "Контакты"],
            anchorColorValue: 'anchor-grey'
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.desktop-nav {
    display: none;
    visibility: hidden;
    font-size: 14px;
    padding: 0;
    margin: 0;

    @media screen and (min-width: 1025px) { display: inline-block; visibility: visible; }

    li:last-child  { padding-right: 0; }
    li:first-child { padding-left: 0; }

    li {
        list-style: none;
        display: inline;
        padding: 0 15px;

            a {
               text-decoration: none;
               line-height: 20px;

               &:hover { text-decoration: underline; }
            }
        }
}
</style>
