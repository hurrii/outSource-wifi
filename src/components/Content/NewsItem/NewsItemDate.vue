<template>
    <time class="news-item__date" datetime="2018-12-05T11:45">05 декабря 2018
        <span><img src="./clock.svg" alt="clock icon svg"></span>   5 мин</time>
</template>

<script>


export default {
  name: 'NewsItemDate'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .news-item__date {
        color: $grey;

        span {
            display: inline-block;
            vertical-align: middle;
            margin-left: 30px;

            @media screen and (max-width: 580px) { margin-left: 20px; }
        }
    }

</style>
