<template>
        <figure class="news-item__carousel">
            <img src="/assets/img/gear-tuning.jpg" class="carousel-img" alt="Настройка оборудования">
            <figcaption id="caption1">Настройка оборудования</figcaption>

            <div class="controls-panel">
                <div class="pic-number">
                    <span class="pic-index">1</span>
                    <span>/</span>
                    <span>3</span>
                </div>
                <figcaption id="caption2">Настройка оборудования</figcaption>
                <div class="carousel-controls" >
                    <span>
                        <svg width="9" height="14" viewBox="0 0 9 14" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M8 1L2 7L8 13" stroke="black" stroke-width="2"/></svg>
                    </span>
                    <span>
                        <svg width="9" height="14" viewBox="0 0 9 14" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M1 1L7 7L1 13" stroke="black" stroke-width="2"/></svg>
                    </span>
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
          margin: 30px 0;
          max-width: 960px;

          #caption1 {
              margin-top: 10px;
              font-size: 14px;
              color: $grey;

                @media screen and (min-width: 768px) {
                    display: none;
                    visibility: hidden;
                }
          }
          #caption2 {
                @media screen and (max-width: 767px) {
                    display: none;
                    visibility: hidden;
                }
          }
        
          .carousel-img {
              display: block;
              max-width: 100%;
              height: auto;
          }

          .controls-panel {
              margin-top: 10px;
              display: flex;
              @media screen and (min-width: 768px) {
                    margin-top: 30px;
              }

            .pic-number { margin-right: 69px; }
                .pic-index { color: $pink }

                .carousel-controls {
                 margin-left: auto;

                    span {
                        width: 6px;
                        height: 12px;
                        cursor: pointer;
                    }

                    span:hover svg path { stroke: $pink; }

                    span:first-child { margin-right: 30px; }
                }
        }
      }
</style>
