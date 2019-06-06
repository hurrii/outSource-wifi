<template>
        <div class="copyright-wrapper">
            <ul>
                <li>© 2018 outSource/wi-fi</li>
                <li>Пользовательское соглашение</li>
            </ul>
        </div>
</template>

<script>


export default {
  name: 'InfoCopyRight'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .copyright-wrapper {

        ul {margin: 0; padding: 20px 0;}

        ul li {
            color: $grey;
            list-style: none;
            padding: 5px 0;
            white-space: nowrap;
        }

        @media screen and (min-width: 768px) {
            ul {
                display: flex;

                li {flex: 0 1 194px;}
            }
        }
    }

</style>
