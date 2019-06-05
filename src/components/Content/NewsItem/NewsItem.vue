<template>
    <article class="news-item">
        <NewsItemHeading/>
        <NewsItemDate/>
        <NewsItemIntroduction/>
        <NewsItemContent/>
    </article>
</template>

<script>
import NewsItemHeading from '@/components/Content/NewsItem/NewsItemHeading.vue'
import NewsItemDate from '@/components/Content/NewsItem/NewsItemDate.vue'
import NewsItemIntroduction from '@/components/Content/NewsItem/NewsItemIntroduction.vue'
import NewsItemContent from '@/components/Content/NewsItem/NewsItemContent.vue'

export default {
  name: 'NewsItem',
  components: {
      NewsItemHeading,
      NewsItemDate,
      NewsItemIntroduction,
      NewsItemContent
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .news-item {
        width: 100%;
        margin: 0 auto;
        
        max-width: 87.5%;

        @media screen and (min-width: 1200px){
            max-width: 960px;
        }
    }
</style>
