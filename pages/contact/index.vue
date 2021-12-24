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
        id="contact__form-email-address"
        type="text"
        class="contact__form-email-address"
      />

      <!-- Message field -->
      <label for="contact__form-msg" class="contact__form-msg-title"
        >Message *</label
      >
      <textarea id="contact__form-msg" type="text" class="contact__form-msg" />
      <input type="submit" class="contact__form-btn" value="submit" />
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
    & input:focus {
      border-color: $primary__color;
    }
    & fieldset,
    &-email-title,
    &-msg-title {
      margin-top: 2.5rem;
    }
    & legend,
    & label {
      font-size: 1.8rem;
      color: black;
      font-weight: 700;
      margin-bottom: 0.5rem;
    }
    &-name-first,
    &-name-last,
    &-phone-first,
    &-phone-second,
    &-phone-third,
    &-email-address,
    &-msg {
      border: 1px solid #ccc;
      background: #fafafa;
      padding: 1.2rem;
      border-radius: 0.2rem;
    }
    &-name {
      display: flex;
      justify-content: center;
      width: 100%;
      &-first,
      &-last {
        width: 50%;
      }
      &-last {
        margin-left: 0.5rem;
      }
    }
    &-phone {
      display: flex;
      &-first,
      &-second,
      &-third {
        width: 25%;
      }
      &-second,
      &-third {
        margin-left: 0.5rem;
      }
    }
    &-msg {
      overflow: auto;
      min-height: 10rem;
      background-clip: padding-box;
    }
    &-btn {
      margin-top: 5rem;
      padding: 1.2rem;
      text-transform: uppercase;
      font-weight: 700;
      width: 50%;
      background-color: $primary__color;
      color: white;
    }
  }
}

//Desktop View
@media (min-width: 1248px) {
  .contact {
    padding: 0 30% 15rem 30%;
    &__title {
      font-size: 6rem;
      line-height: 6rem;
    }
    &__description {
      font-size: 2.5rem;
      line-height: 3.5rem;
    }
    &__form {
      & input,
      textarea {
        font-size: 1.8rem;
      }
      &-btn {
        width: 20%;
        &:hover {
          background: #0af;
          cursor: pointer;
        }
      }
    }
  }
}
</style>
