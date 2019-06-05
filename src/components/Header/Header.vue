<template>
  <header class="header header_shadow">
    <container>
      <div class="row row__first">
        <Logo/>
        <DesktopNav/>
        <MobileNav/>
      </div>
    </container>
    <container>
      <div class="row row__second">
        <Desktop2ndNav/>
        <ContactBlock></ContactBlock>
      </div>
    </container>
      
      
  </header>
</template>

<script>
import Logo from './Logo/Logo.vue'
import Container from '@/components/Container.vue'
import DesktopNav from '@/components/Header/DesktopNav/DesktopNav.vue'
import MobileNav from './MobileNav/MobileNav.vue'
import Desktop2ndNav from '@/components/Header/DesktopNav/Desktop2ndNav.vue'
import ContactBlock from '@/components/Header/ContactBlock/ContactBlock.vue'

export default {
  name: 'Header',
  components: {
    Logo,
    Container,
    DesktopNav,
    Desktop2ndNav,
    ContactBlock,
    MobileNav
  },
    data() {
        return {
            anchors: [
              { message: "Testing"     },
              { message: "This thing"  }
            ]
        }
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
              @media screen and (min-width: 1024px) { border-bottom: 1px solid #E6E6E6; }
            }

            &__second {
              padding: 19px 0 17px;
              @media screen and (max-width: 1024px) { display: none; }
            }
        }
}

</style>
