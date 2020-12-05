<template>
  <footer class="footer">
    <div class="footer__copyright">
      <div class="footer__copyright-social">
        <!-- Twitter Social Icon -->
        <a
          href="http://www.twitter.com/marvthedev"
          class="footer__copyright-social-link"
        >
          <svg
            class="footer__copyright-social-icon footer__copyright-social-icon-twitter"
            viewBox="0 0 250 250"
            xmlns="http://www.w3.org/2000/svg"
            clip-rule="evenodd"
            stroke-linejoin="round"
            stroke-miterlimit="2"
          >
            <path
              d="M229.166 52.081C229.166 23.316 205.85 0 177.084 0 148.316 0 125 23.316 125 52.081v31.25c-45.066 0-85.328-20.465-112.081-52.569C-14.2 90.334 2.787 161.744 55.512 202.444 40.772 215.659 21.341 223.756 0 223.756 23.631 240.253 52.328 250 83.334 250c80.554 0 145.832-65.306 145.832-145.834v-31.25L250 52.081h-20.834zM182.281 62.5c-5.737 0-10.406-4.659-10.406-10.419 0-5.756 4.669-10.415 10.406-10.415 5.76 0 10.428 4.659 10.428 10.415 0 5.76-4.668 10.419-10.428 10.419z"
            />
          </svg>
        </a>

        <!-- Facebook Social Icon -->
        <a
          href="http://www.facebook.com/marvthedev"
          class="footer__copyright-social-link"
        >
          <svg
            class="footer__copyright-social-icon footer__copyright-social-icon-facebook"
            viewBox="0 0 250 250"
            xmlns="http://www.w3.org/2000/svg"
            clip-rule="evenodd"
            stroke-linejoin="round"
            stroke-miterlimit="2"
          >
            <path
              d="M229.166 0H20.834C9.378 0 0 9.378 0 20.834v208.332C0 240.622 9.378 250 20.834 250H125V145.834h-20.834V125H125v-20.834c0-28.766 23.325-52.082 52.084-52.082h20.832v20.832h-20.832c-17.253 0-31.25 13.99-31.25 31.25V125h52.082v20.834h-52.082V250h83.332c11.456 0 20.834-9.378 20.834-20.834V20.834C250 9.378 240.622 0 229.166 0z"
            />
          </svg>
        </a>
      </div>
      <p class="footer__copyright-txt">
        © copyright 2020 Global Orthotics Inc. All Rights Reserved. Website
        designed by
        <a href="https://www.marvthe.dev" class="footer__copyright-link"
          >@marvthedev</a
        >
      </p>
    </div>
  </footer>
</template>

<style lang="scss">
.footer {
  position: relative;
  bottom: 0;
  left: 0;
  padding: 0 5%;
  background: #101c22;
  width: 100%;
  &__copyright {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 1.5rem 0;
    &-link {
      color: $primary__color;
      font-weight: 700;
      cursor: pointer;
      &:hover {
        color: #0af;
      }
    }
    &-social {
      display: flex;
      &-icon {
        cursor: pointer;
        height: 2rem;
        fill: white;
        &-twitter:hover {
          fill: #1da1f2;
        }
        &-facebook:hover {
          fill: #4267b2;
        }
      }
      &-link {
        &:not(:first-child) {
          margin-left: 1rem;
        }
      }
    }
    &-txt {
      margin-top: 1rem;
      font-size: 1.2rem;
      text-align: center;
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
