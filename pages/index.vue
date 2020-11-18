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
      <div class="support__contact">
        <h2 class="support__contact-title">
          Have Questions or Inquiries? <span>Send us a Message!</span>
        </h2>
        form
        <form
          id="support__form"
          class="support__form"
          name="contact"
          method="POST"
          action="/success"
          netlify
          netlify-honeypot="bot-field"
        >
          <input
            type="text"
            placeholder="Your Name"
            name="name"
            class="support__form-input"
          />
          <input
            type="text"
            placeholder="Your Email Address"
            name="email"
            class="support__form-input"
          />
          <input
            type="text"
            placeholder="Subject"
            name="subject"
            class="support__form-input support__form-subject"
          />
          <textarea
            placeholder="How can we help you?"
            name="message"
            class="support__form-msg"
          ></textarea>
        </form>
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
  &__contact {
    height: 100%;
    padding-bottom: 10rem;
    background: #d2deea;
    display: flex;
    flex-direction: column;
    align-items: center;
    &-title {
      padding-top: 6rem;
      font-size: 3.3rem;
      text-align: center;
      & span {
        font-weight: 400;
      }
    }
  }
  &__form {
    width: 100%;
    padding: 0 5%;
    margin-top: 3rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    &-input {
      width: 100%;
      margin: 0.5rem 0;
      padding: 1rem;
      font-size: 1.6rem;
      border: 0.1rem solid #d9d9d9;
      &:focus {
        outline: none;
        border: 0.3rem solid #0088cc;
      }
    }
    &-subject {
      margin-top: 2rem;
    }
    &-msg {
      margin-top: 0.5rem;
      height: 25rem;
      width: 100%;
      padding: 1rem;
      font-size: 1.6rem;
    }
  }
}
</style>
