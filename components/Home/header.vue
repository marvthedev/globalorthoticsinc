<template>
  <header class="header">
    <div class="header__txt">
      <h1 class="header__txt-title">
        Global Orthotics Inc.
        <span class="header__sub-head"
          >creates a wide variety of custom made Orthotics in Ontario.</span
        >
      </h1>
      <p class="header__txt-excerpt">
        Our Orthotics are designed to create functional correction, regain foot
        mechanical advantage, improve stability, and overall posture and
        alignment.
      </p>
      <nuxt-link to="/about" class="header__txt-btn">About Us</nuxt-link>
    </div>
    <img src="~/assets/svg/header/header-business.svg" class="header__img" />
  </header>
</template>

<style lang="scss">
.header {
  margin-top: 16rem;
  display: flex;
  flex-direction: column;
  width: 100%;
  &__txt {
    display: flex;
    flex-direction: column;
    &-title {
      width: 90%;
      font-size: 3.3rem;
      line-height: 3.3rem;
    }
    &-excerpt {
      margin: 4.5rem 0;
    }
    &-btn {
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
  }
  &__img {
    height: 20rem;
  }
  &__sub-head {
    font-size: 3rem;
    font-weight: 300;
  }
  &__img {
    margin-top: 3rem;
    width: 100%;
  }
}

//Desktop view
@media (min-width: 1248px) {
  .header {
    flex-direction: row;
    align-items: center;
    padding: 0 15.4rem;
    &__txt {
      &-btn {
        width: 30%;
      }
    }
    &__img {
      height: 40rem;
    }
  }
}
</style>
