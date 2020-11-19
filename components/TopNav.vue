<template>
  <nav class="nav">
    <div class="nav__container">
      <div class="nav__logo">
        <img
          src="~/assets/svg/nav/global-orthotics-inc-logo.svg"
          class="nav__logo-img"
        />
      </div>
      <div class="nav__toggle">
        <svg
          class="nav__toggle-bars"
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 448 512"
        >
          <path
            d="M436 124H12c-6.627 0-12-5.373-12-12V80c0-6.627 5.373-12 12-12h424c6.627 0 12 5.373 12 12v32c0 6.627-5.373 12-12 12zm0 160H12c-6.627 0-12-5.373-12-12v-32c0-6.627 5.373-12 12-12h424c6.627 0 12 5.373 12 12v32c0 6.627-5.373 12-12 12zm0 160H12c-6.627 0-12-5.373-12-12v-32c0-6.627 5.373-12 12-12h424c6.627 0 12 5.373 12 12v32c0 6.627-5.373 12-12 12z"
          />
        </svg>
      </div>
    </div>
    <div class="nav__menu">
      <nuxt-link to="/home" class="nav__menu-link">Home</nuxt-link>
      <nuxt-link to="/about" class="nav__menu-link">About</nuxt-link>
      <nuxt-link to="/home" class="nav__menu-link">Orthotics</nuxt-link>
    </div>
  </nav>
</template>

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
    background: $primary__color;
    padding: 0.7rem 1.3rem;
    height: 3.4rem;
    border-radius: 0.25rem;
    cursor: pointer;
    &-bars {
      width: 1.2rem;
      fill: white;
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
