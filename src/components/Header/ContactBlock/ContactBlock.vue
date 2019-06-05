<template>
    <div class="header__contact-block contact-block">
        <ContactPhone/>
        <ContactSendAppl/>
    </div>
</template>

<script>
import ContactPhone from './ContactPhone.vue'
import ContactSendAppl from './ContactSendAppl.vue'

export default {
    name: 'ContactBlock',
    components: {
        ContactPhone,
        ContactSendAppl
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
        .contact-block {
            white-space: nowrap;
        }
</style>
