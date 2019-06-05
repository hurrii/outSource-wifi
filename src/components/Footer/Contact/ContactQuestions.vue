<template>
        <div class="contact-questions">
            <div class="wrapper">
                
            <h2>Ответим на ваши вопросы</h2>
            <p>Каждый день мы меняем мир к лучшему, присоединяйтесь</p>
            </div>
        </div>
</template>

<script>

export default {
  name: 'ContactQuestions',
  components: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .contact-questions {
        max-width: 100%;
        flex-basis: 374px;
        flex: 1;

        .wrapper {
            max-width: 340px;
        }

            h2 {
                margin: 0;
                color: #FFFFFF;
                padding-bottom: 55px;
                font-size: 26px;
                    @media screen and (min-width: 768px) { font-size: 40px; padding-bottom: 20px;}
            }

            p {
                margin: 0;
                font-size: 16px;
                    @media screen and (max-width: 768px) { display: none; visibility: hidden; }
            }
    }
</style>
