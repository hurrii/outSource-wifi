<template>
  <header class="header header_shadow">
    <container>
      <div class="row">
        <Logo/>
        <DesktopNav/>
        <MobileNav/>
      </div>
    </container>
    <container>
      <DesktopNav/>
    </container>
      
      
  </header>
</template>

<script>
import Logo from './Logo/Logo.vue'
import Container from '@/components/Container.vue'
import DesktopNav from '@/components/Header/DesktopNav/DesktopNav.vue'
import MobileNav from './MobileNav/MobileNav.vue'

export default {
  name: 'Header',
  components: {
    Logo,
    Container,
    DesktopNav,
    MobileNav
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .header {
        color: $black;
        background: $white;

        &_shadow {
          box-shadow: 0 5px 15px 0 rgba(0, 0, 0, 0.1);
        }

        .row {
          display: flex;
          width: 100%;
          justify-content: space-between;
          align-items: center;
          padding: 18px 0;

          @media screen and (min-width: 1160px) {
                  border-bottom: 1px solid #E6E6E6;
          }
      }


    
}

</style>
