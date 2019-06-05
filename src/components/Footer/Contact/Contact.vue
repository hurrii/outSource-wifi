<template>
        <section class="contact">
            <div class="row">
                <ContactQuestions/>
                <ContactSendQuestion/>
            </div>
        </section>
</template>

<script>
import ContactQuestions from './ContactQuestions.vue'
import ContactSendQuestion from './ContactSendQuestion.vue'

export default {
  name: 'Contact',
  components: {
      ContactQuestions,
      ContactSendQuestion
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .contact {
        background: #202E35;
        color: $grey;
        padding: 80px 0;
    }

        .row {
            max-width: 87.5%;
            display: flex;
            flex-direction: column;
            margin: 0 auto;
            

                @media screen and (min-width: 360px) {max-width: 87.5%;}
                @media screen and (min-width: 768px) {flex-direction: row;}
                @media screen and (min-width: 1440px) {max-width: 1160px;}
            }
</style>
