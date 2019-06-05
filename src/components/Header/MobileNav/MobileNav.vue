<template>
    <div class="header__mobile-nav mobile-nav">
        <button class="mobile-nav__button mobile-nav__phone-icon"></button>
        <button class="mobile-nav__button mobile-nav__burger-icon"></button>
    </div>
</template>

<script>

export default {
  name: 'MobileNav'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.mobile-nav {
    display: inline-block;

    @media screen and (min-width: 1025px) {
        visibility: hidden;
        display: none;
    }

    &__button {
        display: inline-block;
        width: 16px;
        height: 16px;
        border: 0;
        padding: 0;
        cursor: pointer;
    }

    &__phone-icon {
        background: url('./phone-icon.svg') no-repeat;
        background-size: cover;
        margin-right: 20px;
    }
    &__burger-icon {
        background: url('./burger-menu.svg') no-repeat;
        background-size: cover;
    }
}
</style>
