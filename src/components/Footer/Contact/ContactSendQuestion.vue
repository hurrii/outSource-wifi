<template>
    <div class="send-question">
        <form action="" class="contact-form">
            <div class="text-tel-wrapper">
                <input type="text" name="name" id="contact-name" placeholder="Имя" onfocus="this.placeholder = ''" onblur="this.placeholder = 'Имя'">
                <div class="divider"></div>
                <input type="tel" name="phone" id="contact-phone" placeholder="Телефон" onfocus="this.placeholder = ''" onblur="this.placeholder = 'Телефон'">
            </div>
            <input type="text" name="message" id="contact-msg" placeholder="Сообщение" onfocus="this.placeholder = ''" onblur="this.placeholder = 'Сообщение'">
            
            <div class="submit-wrapper">
                <span>Нажимая на кнопку, вы даете согласие на обработку персональных данных и соглашаетесь с политикой конфиденциальности
                </span>
                <button type="submit">Отправить</button>
            </div>
        </form>
    </div>
</template>

<script>

export default {
  name: 'ContactSendQuestion'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .send-question {
        flex: 1;
        width: 100%;
        max-width: 560px;
        overflow: hidden;
    }

    .contact-form {
        display: flex;
        flex-wrap: wrap;
        

        input {
            border: 0;
            flex: 1;
            min-height: 44px;
            background: none;
            border-bottom: 1px solid $grey;
            color: $grey;
        }

    }

        .text-tel-wrapper {
            flex: 1 1 100%;
            display: flex;
            flex-wrap: wrap;
            padding-bottom: 60px;

            @media screen and (max-width: 1023px) { flex-direction: column; }
            
            .divider {
                flex-basis: 40px;
                max-width: 40px;
                flex: 1;
                @media screen and (max-width: 1023px) {
                    display: none; visibility: hidden;
                }
            }
            input { flex-basis: 260px; flex: 1; }
        }


        .submit-wrapper {
            flex-basis: 560px;
            width: 100%;
            display: flex;
            align-items: center;
            padding-top: 37px;
            flex-wrap: wrap;

            span {
                flex-basis: 319px;
                width: 319px;
                flex: 1;
                padding-right: 24px;
                @media screen and (max-width: 580px) { font-size: 13px }
            }


            button {
                border: 0;
                max-width: 216px;
                flex-basis: 216px;
                background: $pink;
                color: $white;
                border-radius: 2px;
                height: 48px;
                flex: 1;
                cursor: pointer;
            }

            @media screen and (max-width: 1024px) {
                span {order: 2; flex-basis: 100%; padding-top: 10px;}
                button {order: 1; flex-basis: 100%; }
            }
        }

        
</style>
