<template>
        <figure class="news-item__carousel">
            <img src="/assets/img/gear-tuning.jpg" alt="Настройка оборудования">

            <div class="controls-panel">
                <div class="pic-number">
                    <span class="pic-index">1</span>
                    <span>/</span>
                    <span>3</span>
                </div>
                <figcaption>Настройка оборудования</figcaption>
                <div class="carousel-controls">
                    <span><img src="./chevron-left.svg" alt="clock icon svg"></span>
                    <span><img src="./chevron-right.svg" alt="clock icon svg"></span>
                </div>
                
            </div>
        </figure>
</template>

<script>

export default {
  name: 'NewsItemCarousel'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
      .news-item__carousel {

          .controls-panel {
              display: flex;

              .pic-number {
                  .pic-index {color: $pink}
              }
          }

          figure {
              margin: 0;

              img {
                  display: block;
                  max-width: 100%;
                  height: auto;
              }
          }
      }
</style>
