<template>
  <div class="index">
    <topNav class="wrapper" />
    <homeHeader class="wrapper" />
    <section class="support">
      <h2 class="support__heading">
        Our Orthotics are designed to create functional correction, regain foot
        mechanical advantage, improve stability, and overall posture and
        alignment.
      </h2>
      <img src="~/assets/svg/support/support.svg" class="support__img" />
      <div class="support__form">
        <h2>Send us a Message!</h2>
      </div>
    </section>
  </div>
</template>

<script>
import topNav from '~/components/TopNav'
import homeHeader from '~/components/Home/header'

export default {
  components: {
    topNav,
    homeHeader
  }
}
</script>

<style lang="scss">
.wrapper {
  padding: 0 5%;
}
.support {
  width: 100%;
  max-height: 100%;
  font-size: 0;
  &__img {
    z-index: -1;
    width: 100%;
  }
  &__heading {
    margin-left: 5%;
    width: 65%;
    line-height: 2.3rem;
    position: relative;
    top: 14.5rem;
    font-size: 1.7rem;
  }
  &__form {
    height: 20rem;
    background: #d2deea;
  }
}
</style>
