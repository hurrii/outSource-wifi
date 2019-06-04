<template>
    <div class="header__mobile-nav mobile-nav">
        <button class="mobile-nav__button mobile-nav__phone-icon"></button>
        <button class="mobile-nav__button mobile-nav__burger-icon"></button>
    </div>
</template>

<script>
// eslint-disable-next-line
import BurgerMenu from './burger-menu.svg';
// eslint-disable-next-line
import PhoneIcon from './phone-icon.svg';

export default {
  name: 'MobileNav'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.mobile-nav {
    display: inline-block;

    @media screen and (min-width: 1024px) {
        visibility: hidden;
        display: none;
    }

    &__button {
        display: inline-block;
        margin-right: 20px;
        width: 16px;
        height: 16px;
        border: 0;
        padding: 0;
        cursor: pointer;
    }

    &__phone-icon {
        background: url('./phone-icon.svg') no-repeat;
        background-size: cover;
    }
    &__burger-icon {
        background: url('./burger-menu.svg') no-repeat;
        background-size: cover;
    }
}
</style>
