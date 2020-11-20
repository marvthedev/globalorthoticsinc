<template>
  <nav class="nav">
    <div class="nav__container">
      <div class="nav__logo">
        <img
          src="~/assets/svg/nav/global-orthotics-inc-logo.svg"
          class="nav__logo-img"
        />
      </div>
      <div class="nav__toggle" @click="menuOpened = true">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>
    <div v-show="menuOpened" class="nav__menu">
      <nuxt-link to="/home" class="nav__menu-link">Home</nuxt-link>
      <nuxt-link to="/about" class="nav__menu-link">About</nuxt-link>
      <nuxt-link to="/home" class="nav__menu-link">Orthotics</nuxt-link>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      menuOpened: false
    }
  }
}
</script>

<style lang="scss">
.nav {
  margin-top: 1.5rem;
  display: flex;
  flex-direction: column;
  &__container {
    display: flex;
    justify-content: space-between;
    width: 100%;
  }
  &__logo {
    &-img {
      height: 4rem;
    }
  }
  &__toggle {
    display: flex;
    flex-direction: column;
    height: 50%;
    background: $primary__color;
    padding: 0.7rem 1rem;
    border-radius: 0.25rem;
    cursor: pointer;
    & span {
      background: white;
      width: 1.1rem;
      height: 0.2rem;
      margin: 0.12rem 0;
      transition: all 0.4s ease;
      transform-origin: 0 0;
    }
  }
  &__menu {
    margin-top: 2rem;
    width: 100%;
    display: flex;
    flex-direction: column;
    padding: 0 2rem;
    &-link {
      font-size: 1.2rem;
      text-transform: uppercase;
      font-weight: 700;
      padding: 1rem;
      border-bottom: 0.1rem solid #777;
      color: $primary__color;
      &-hover {
        background: $primary__color;
        color: white;
      }
    }
  }
}
//Desktop View
@media (min-width: 1248px) {
  .nav {
    &__toggle {
      display: none;
    }
  }
}
</style>
