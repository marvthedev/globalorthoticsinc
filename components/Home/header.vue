<template>
  <header class="header">
    <h1 class="header__title">
      Global Orthotics Inc.
      <span class="header__sub-head"
        >creates a wide variety of custom made Orthotics in Ontario.</span
      >
    </h1>
    <p class="header__excerpt">
      Our Orthotics are designed to create functional correction, regain foot
      mechanical advantage, improve stability, and overall posture and
      alignment.
    </p>
    <nuxt-link to="/about" class="header__btn">About Us</nuxt-link>
  </header>
</template>

<style lang="scss">
.header {
  margin-top: 9rem;
  display: flex;
  flex-direction: column;
  width: 100%;
  &__title {
    width: 90%;
    font-size: 3.3rem;
    line-height: 3.3rem;
  }
  &__sub-head {
    font-size: 3rem;
    font-weight: 300;
  }
  &__excerpt {
    margin: 6rem 0 3rem 0;
  }
  &__btn {
    width: 45%;
    text-align: center;
    padding: 1.1rem 3.6rem;
    border: 0.2rem solid $primary__color;
    border-radius: 2rem;
    font-size: 1.6rem;
    font-weight: 700;
    color: $primary__color;
    text-decoration: none;
  }
  &__img {
    margin-top: 3rem;
    width: 100%;
  }
}
</style>
