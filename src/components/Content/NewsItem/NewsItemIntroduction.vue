<template>
    <span class="news-item__intro">
        <h2>Компания «outSource/wi-fi» построила беспроводную Wi-Fi-сеть в торгово-производственном холдинге «Росатом».
        Теперь Wi-Fi могут пользоваться 3 тысячи сотрудников «Росатома» одновременно. «outSource/wi-fi»
        также организовал сеть Wi-Fi на Ижевском заводе тепловой техники (ИЗТТ), который принадлежит холдингу.
        </h2>
    </span>
</template>

<script>


export default {
  name: 'NewsItemIntroduction'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
      .news-item__intro {
          margin: 40px 0;
          @media screen and (min-width: 580px) { margin: 60px 0; }
      }
</style>
