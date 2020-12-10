<template>
  <div class="contact">
    <h1 class="contact__title">
      Have questions? <span>Send us a message.</span>
    </h1>
    <p class="contact__description">
      Use the form below if you have any questions or would like to book an
      appointment. All replies from us will be done during business hours.
    </p>
    <form class="contact__form">
      <fieldset class="contact__form-name">
        <!-- First and last name fields -->
        <legend class="contact__form-name-title">Name *</legend>
        <input type="text" class="contact__form-name-first" />
        <input type="text" class="contact__form-name-last" />
      </fieldset>

      <!-- Phone Number Fields -->
      <fieldset class="contact__form-phone">
        <legend class="contact__form-phone-title">Phone Number *</legend>
        <input type="text" class="contact__form-phone-first" />
        <input type="text" class="contact__form-phone-second" />
        <input type="text" class="contact__form-phone-third" />
      </fieldset>

      <!-- Email address field -->
      <label for="contact__form-email-address" class="contact__form-email-title"
        >Email *</label
      >
      <input
        type="text"
        id="contact__form-email-address"
        class="contact__form-email-address"
      />

      <!-- Message field -->
      <label for="contact__form-message" class="contact__form-message-title"
        >Message *</label
      >
      <textarea
        type="text"
        id="contact__form-message"
        class="contact__form-message"
      />
    </form>
  </div>
</template>

<style lang="scss">
.contact {
  display: flex;
  flex-direction: column;
  min-height: 90vh;
  padding: 0 4% 10rem 4%;
  &__title {
    margin-top: 16rem;
    font-size: 3.2rem;
    width: 85%;
    line-height: 3rem;
    & span {
      font-weight: 400;
    }
  }
  &__description {
    margin-top: 3rem;
  }
  &__form {
    margin-top: 3rem;
    display: flex;
    flex-direction: column;
    width: 100%;
    & fieldset,
    &-email-title,
    &-message-title {
      margin-top: 2.5rem;
    }
    & legend,
    & label {
      font-size: 1.8rem;
      color: black;
      font-weight: 700;
    }
    & input,
    & textarea {
      border: 1px solid #ccc;
      background: #fafafa;
      padding: 1.2rem 1.2rem;
      margin-top: 0.5rem;
      border-radius: 0.2rem;
    }
    &-name {
      display: flex;
      justify-content: center;
      width: 100%;
      &-first,
      &-last {
        margin: 0 0.5rem;
        width: 50%;
      }
    }
    &-phone {
      display: flex;
      &-first,
      &-second,
      &-third {
        margin: 0 0.5rem;
        width: 25%;
      }
    }
    &-message {
      overflow: auto;
      min-height: 10rem;
      background-clip: padding-box;
    }
  }
}
</style>
