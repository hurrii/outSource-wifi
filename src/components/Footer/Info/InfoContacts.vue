<template>
        <nav class="info-contacts">
            
            <LogoFooter/>
            <address class="firm-address">
                Москва, Волоколамское шоссе 10, офис 22
                <a class="map-link" href="https://yandex.ru/maps/-/CCCHiCY-">
                    Смотреть на карте
                </a>
            </address>
                

                <address class="firm-contacts">
                    <a href="tel:+74877340123">+7 (487) 734-01-23</a>
                    <a href="mailto:wi-fi@outsource.ru">wi-fi@outsource.ru</a>
                    <a href="http://facebook.com">facebook</a>
                </address>
        </nav>
</template>

<script>
import LogoFooter from '@/components/Logo/LogoFooter.vue'


export default {
  name: 'InfoContacts',
  components: {
      LogoFooter
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .info-contacts {
        flex: 1 1 172px;
        width: 100%;
        display: flex;
        border-bottom: 1px solid $grey;
        padding: 40px 0;
        align-items: baseline;
        flex-wrap: wrap;

        address {
            display: flex;
            font-style: normal;
            flex: 0 1 100%;
            padding: 15px 0;

            .map-link { color: $grey; }

            a {
            text-decoration: none;
            color: $white;
            flex: 1;
            padding: 10px 0;
            }

            a:hover { color: $pink; }
        }

        .firm-address {
            flex-direction: column;
        }

        .firm-contacts {
            white-space: nowrap;
            flex-direction: column;
            justify-content: space-between;
    }
}

// 768px and larger

.info-contacts {

@media screen and (min-width: 768px) {
    
    flex-wrap: nowrap;

    address {
        padding: 0;
        flex-direction: row;
        flex: 0 1 45%;
    }

    .firm-contacts {
        flex-direction: row;
        justify-content: space-between;
            
            a { padding: 0 5px; }
            a:nth-child(3) { text-align: right; }
    }
 }
}
</style>
