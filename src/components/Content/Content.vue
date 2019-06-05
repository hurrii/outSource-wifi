<template>
    <main class="content">
        <Container>
          <OnPageNav/>
        </Container>
        <NewsItem/>
    </main>
</template>

<script>
import Container from '@/components/Container.vue'
import OnPageNav from '@/components/Content/OnPageNav/OnPageNav.vue'
import NewsItem from '@/components/Content/NewsItem/NewsItem.vue'

export default {
  name: 'Header',
  components: {
      Container,
      OnPageNav,
      NewsItem
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .header {
        color: $black;

        &_shadow { box-shadow: 0 5px 15px 0 rgba(0, 0, 0, 0.1); }

        .row {
            display: flex;
            width: 100%;
            justify-content: space-between;
            align-items: center;

            &__first {
              padding: 23px 0 17px;
              @media screen and (min-width: 768px) { border-bottom: 1px solid #E6E6E6; }
            }

            &__second {
              padding: 19px 0 17px;
              @media screen and (max-width: 767px) { display: none; }
            }
        }
}

</style>
