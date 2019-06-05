<template>
    <div class="news-item__content">
        <div class="text-block">
            <p>
                «Росатом» с 1996 года производит климатическую и инженерную технику, предоставляет услуги по ее проектированию, монтажу, поставки и сервисному обслуживанию. Помимо России, холдинг ведет свою деятельность в странах СНГ и Балтии.
            </p>
        <p>
            До проекта в «Росатоме» работала Wi-Fi-сеть, но её скорость не позволяла сотрудникам холдинга быстро обмениваться данными через Интернет. Соединение порой резко обрывалось, что создавало сложности в общении сотрудников «Росатома» с клиентами в режиме онлайн.
        </p>
        </div>

        <figure>
            <img src="/assets/img/objects-radioexploring.jpg"/>
            <figcaption>Радиообследование объектов</figcaption>
        </figure>
        
        <div class="text-block">
            <p>
                «Росатому» требовалась бесперебойная и высокоскоростная Wi-Fi-сеть. Для ее создания были приглашены специалисты outSource/wi-fi. Им нужно было развернуть Wi-Fi-сеть в офисе общей площадью 9 500 м2 и учесть все требования холдинга по безопасности и отказоустойчивости сети.
            </p>
            <p>
                Специалисты outSource/wi-fi провели работы по проектированию беспроводной сети, ее настройке и тестированию. Проектирование беспроводной сети выполнено на основе данных, которые были получены в результате проведённой процедуры SiteSurvey в типовых областях и комплексного моделирования с помощью специализированного ПО.
            </p>
        </div>

        <NewsItemCarousel/>

        <div class="text-block">
            <p>
                Специалисты компании провели работы по проектированию беспроводной сети, ее настройке и тестированию. Проектирование беспроводной сети выполнено на основе данных, которые были получены в результате проведённой процедуры SiteSurvey в типовых областях и комплексного моделирования с помощью специализированного ПО.
            </p>
        </div>
    </div>
</template>

<script>
import NewsItemCarousel from './NewsItemCarousel.vue'

export default {
  name: 'NewsItemContent',
  components: {
      NewsItemCarousel
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
      .news-item__content {
          // margin: 40px 0;
          // @media screen and (min-width: 580px) { margin: 60px 0; }

          p {
              margin: 30px 0;
              color: $grey;
          }

          figure {
              margin: 0;

              img {
                  display: block;
                  max-width: 100%;
                  height: auto;
              }

              figcaption {
                  margin-top: 20px;
                  color: 16px;
                  color: $grey;
              }
          }
      }
</style>
