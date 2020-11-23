<template>
  <section class="form">
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
  </section>
</template>

<style lang="scss">
.support {
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
        border: 0.3rem solid $primary__color;
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
      &:focus {
        outline: none;
        border: 0.3rem solid $primary__color;
      }
    }
  }
}
</style>
