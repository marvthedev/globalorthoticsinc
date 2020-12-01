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
    <div class="header__img">
      <img src="~/assets/svg/header/header-business.svg" />
    </div>
  </header>
</template>

<style lang="scss">
.header {
  margin-top: 16rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  &__txt {
    display: flex;
    flex-direction: column;
    &-title {
      font-size: 3.3rem;
      line-height: 3.3rem;
    }
    &-excerpt {
      margin: 4.5rem 0;
    }
    &-btn {
      width: 50%;
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
    margin-top: 6rem;
    display: flex;
    & img {
      width: 100%;
    }
  }
  &__sub-head {
    font-size: 3rem;
    font-weight: 300;
  }
}

//Desktop view
@media (min-width: 1248px) {
  .header {
    flex-direction: row;
    align-items: center;
    padding: 0 15.4rem;
    &__txt {
      padding-left: 7%;
      width: 50%;
      &-btn {
        width: 30%;
        &:hover {
          color: white;
          background: $primary__color;
        }
      }
    }
    &__img {
      padding-right: 4%;
      height: 100%;
      width: 60%;
      color: crimson;
      & img {
        height: 50rem;
      }
    }
  }
}
</style>
