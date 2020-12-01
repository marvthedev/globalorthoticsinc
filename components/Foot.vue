<template>
  <footer class="footer">
    <div class="footer__copyright">
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
      <p class="footer__copyright-txt">
        © copyright 2020. All Rights Reserved. Website designed by
        <a href="https://www.marvthe.dev" class="footer__copyright-link"
          >@marvthedev</a
        >
      </p>
    </div>
  </footer>
</template>

<style lang="scss">
.footer {
  padding: 0 5%;
  background: #101c22;
  &__copyright {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 1.5rem 0;
    &-link {
      color: $primary__color;
      font-weight: 700;
      cursor: pointer;
    }
    &-social {
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
    &-txt {
      margin-top: 1rem;
      font-size: 1rem;
    }
  }
}

//Desktop view
@media (min-width: 1248px) {
  .footer {
    &__copyright {
      padding: 3rem 0;
      &-txt {
        font-size: 1.5rem;
      }
    }
  }
}
</style>
