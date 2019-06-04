<template>
    <ul class="header__desktop-nav desktop-nav">
        <li>
            <linkAnchor anchorText="О компании"  anchorColor="anchor-grey"/>
        </li>
        <li>
            <linkAnchor anchorText="Проекты" anchorColor="anchor-grey"/>
        </li>
        <li>
            <linkAnchor anchorText="Новости" anchorColor="anchor-grey"/>
        </li>
        <li>
            <linkAnchor anchorText="Контакты" anchorColor="anchor-grey"/>
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
    props: {
        customLinkText: Array
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
    padding-right: 5px;

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

        

        a {
            text-decoration: none;
            color: {}

            &:hover {
                text-decoration: underline;
            }
        }
    }
}
</style>
