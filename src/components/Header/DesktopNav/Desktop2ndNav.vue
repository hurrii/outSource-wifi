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
            anchorTextValue: ["Продукты", "Услуги", "Отраслевые решения", "Программное обеспечение"],
            anchorColorValue: 'anchor-black'
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.desktop-nav {
    display: none;
    visibility: hidden;
    padding: 0;
    margin: 0;
    white-space: nowrap;

    @media screen and (min-width: 1024px){
        display: inline-block;
        visibility: visible;
    }

    li:last-child {
        padding-right: 0;
    }

    li:first-child {
        padding-left: 0;
    }

    li {
        list-style: none;
        display: inline;
        padding: 0 15px;

        @media screen and (min-width: 1024px) { padding: 0 8px; }

        a {
            text-decoration: none;
            line-height: 20px;

            &:hover {
                color: $pink;
            }
        }
    }
}
</style>
