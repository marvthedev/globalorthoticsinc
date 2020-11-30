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
        <nuxt-link to="/about" class="support__contact-btn"
          ><img
            src="~/assets/svg/support/message.svg"
            class="support__contact-btn-img"
          />Send a Message</nuxt-link
        >
        <div class="support__email">
          <img
            src="~/assets/svg/support/email.svg"
            class="support__email-img"
          />
          <div class="support__email-txt">
            <h2>Send an email</h2>
            <a href="mailto:marvthedev@gmail.com" class="support__email-address"
              >marvthedev@gmail.com</a
            >
          </div>
        </div>
        <div class="support__call">
          <img src="~/assets/svg/support/call.svg" class="support__call-img" />
          <div class="support__call-txt">
            <h2>Give us a call</h2>
            <a href="mailto:marvthedev@gmail.com" class="support__call-number"
              >(416) 297-0550</a
            >
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
    top: 3.2rem;
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
    padding: 0 5% 10rem 5%;
    background: #d2deea;
    display: flex;
    flex-direction: column;
    justify-content: center;

    &-heading {
      padding-top: 6rem;
      font-size: 3.3rem;
      & span {
        font-weight: 400;
      }
    }
    &-btn {
      margin: 3rem auto 0 auto;
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
  &__email {
    display: flex;
    align-items: center;
    margin-top: 3rem;
    &-img {
      height: 4rem;
    }
    &-txt {
      margin-left: 2rem;
      font-size: 1.4rem;
    }
    &-address {
      cursor: pointer;
      font-size: 2.3rem;
      color: $primary__color;
    }
  }
  &__call {
    display: flex;
    align-items: center;
    margin-top: 3rem;
    &-img {
      margin-left: 2.3rem;
      height: 6rem;
    }
    &-txt {
      margin-left: 2rem;
      font-size: 1.4rem;
    }
    &-number {
      cursor: pointer;
      font-size: 2.3rem;
      color: $primary__color;
    }
  }
}

//Desktop view
@media (min-width: 1248px) {
  .wrapper {
    padding: 0 15.4rem;
  }
}
</style>
