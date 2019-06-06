<template>
        <ul class="onpage-nav">
            <li>
                <a href="#">Главная</a>
            </li>
            <li>
                <a href="#">О компании</a>
            </li>
            <li>
                <a href="#">Новости</a>
            </li>
            <li>
                <a href="#">outSource/wi-fi построил Wi-Fi сеть «Росатому» и ИЗТТ</a>
            </li>
        </ul>
</template>

<script>

export default {
    name: 'OnPageNav'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.onpage-nav {
    display: none;
    visibility: hidden;
    padding: 0;
    margin: 40px 0 0;

    @media screen and (min-width: 768px) { display: block; visibility: visible; }

    li:last-child  { padding-right: 0; }
    li:first-child { padding-left: 0; }

    li {
        list-style: none;
        display: inline;

            a {
                color: rgba(0, 0, 0, 0.4);
                text-decoration: none;
                font-size: 14px;

                    &:hover { text-decoration: underline; }
              }
        }

        li::after {
        content: '/';
        font-family: initial;
        padding: 0 4px;
    }

        li:last-child::after {
            content: '';
            padding-right: 0;
        }
}
</style>
