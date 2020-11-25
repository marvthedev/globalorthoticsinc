<template>
  <footer class="footer">
    <div class="footer__copyright">
      <p class="footer__copyright-txt">
        © copyright 2020. All Rights Reserved. Website designed by
        <a href="https://www.marvthe.dev>" class="footer__copyright-link"
          >@marvthedev</a
        >
      </p>
      <div class="footer__copyright-social">
        <a
          href="http://www.twitter.com/marvthedev"
          class="footer__copyright-social-link"
        >
          <img
            src="~/assets/svg/footer/twitter.svg"
            class="footer__copyright-social-icon"
          />
        </a>
        <a
          href="http://www.facebook.com/marvthedev"
          class="footer__copyright-social-link"
        >
          <img
            src="~/assets/svg/footer/facebook.svg"
            class="footer__copyright-social-icon"
          />
        </a>
      </div>
    </div>
  </footer>
</template>

<style lang="scss">
.footer {
  padding: 0 5%;
  background: #101c22;
  &__copyright {
    padding: 1.5rem 0;
    &-txt {
      font-size: 1rem;
    }
    &-link {
      color: $primary__color;
      font-weight: 700;
      cursor: pointer;
    }
    &-social {
      margin-top: 2rem;
      display: flex;
      &-icon {
        cursor: pointer;
        height: 2rem;
      }
      &-link {
        &:not(:first-child) {
          margin-left: 1rem;
        }
      }
    }
  }
}
</style>
