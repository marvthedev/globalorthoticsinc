<template>
  <div class="index">
    <topNav class="wrapper" />
    <homeHeader class="wrapper" />
    <section class="support">
      <h2 class="support__heading">
        Over 20 years of experience
        <span>in manufacturing Orthotics that suit your needs.</span>
      </h2>
      <img src="~/assets/svg/support/support.svg" class="support__img" />
      <div class="support__contact">
        <h2 class="support__contact-heading">
          Have Questions or Inquiries? <span>Get in touch with us today!</span>
        </h2>
        <div class="support__email">
          <img
            src="~/assets/svg/support/email.svg"
            class="support__email-img"
          />
          <div class="support__email-txt">
            <h2>Email Us</h2>
            <a href="mailto:marvthedev@gmail.com">marvthedev@gmail.com</a>
          </div>
        </div>
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
  margin-top: 6rem;
  width: 100%;
  font-size: 0;
  &__heading {
    z-index: -1;
    margin-left: 5%;
    width: 90%;
    line-height: 3.3rem;
    position: relative;
    top: 3.5rem;
    font-size: 2.2rem;
    & span {
      font-weight: 400;
    }
    &__img {
      z-index: -1;
      width: 100%;
    }
  }
  &__contact {
    height: 100%;
    padding-bottom: 10rem;
    background: #d2deea;
    display: flex;
    flex-direction: column;
    align-items: center;
    &-heading {
      padding-top: 6rem;
      font-size: 3.3rem;
      text-align: center;
      & span {
        font-weight: 400;
      }
    }
  }
  &__email {
    display: flex;
    justify-content: center;
    &-img {
      height: 4rem;
    }
  }
}
</style>
