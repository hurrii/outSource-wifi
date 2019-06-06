<template>
    <section class="info">
        <Container>
            <InfoContacts/>
            <InfoCopyRight/>
        </Container>
    </section>
</template>

<script>
import Container from '@/components/Container.vue'
import InfoContacts from '@/components/Footer/Info/InfoContacts.vue'
import InfoCopyRight from '@/components/Footer/Info/InfoCopyRight.vue'

export default {
  name: 'Info',
  components: {
      Container,
      InfoContacts,
      InfoCopyRight
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .info {
        display: flex;
        background: #05151D;
        color: $white;
    }
</style>
