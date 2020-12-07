<template>
  <div class="orthotics">
    <img src="~/assets/img/orthotics/feet-walk.jpg" class="orthotics__img" />
    <div class="orthotics__txt">
      <h2 class="orthotics__txt-title">Orthotics: What are they?</h2>
      <p>
        Orthotics are customized footwear inserts that is prescribed by a
        doctor. It is specifically made for the individual to treat foot, leg or
        back problems.
      </p>
      <h2 class="orthotics__txt-title">What Problems Can Orthotics Fix?</h2>
      <p>
        Doctors can prescribe Orthotics that can fix some of the following
        problems:
      </p>
      <ul class="orthotics__txt-list">
        <li class="orthotics__txt-list-item">
          <img
            src="~/assets/img/orthotics/check-icon.svg"
            class="orthotics__txt-list-item-icon"
          />
          <p>
            <span>Arthritis.</span> Orthotics can treat discomfort in the feet
            and correct poor positioning.
          </p>
        </li>
        <li class="orthotics__txt-list-item">
          <img
            src="~/assets/img/orthotics/check-icon.svg"
            class="orthotics__txt-list-item-icon"
          />
          <p>
            <span>Back pain.</span> Poor foot positioning, such as
            inward-rolling arches, or poor cushioning can cause lower back pain.
            Orthotics can provide cushioning and correct arches to lessen this
            pain.
          </p>
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss">
.orthotics {
  margin: 10rem 0 5rem 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  min-height: 90vh;
  width: 100%;
  padding: 0 4%;
  &__img {
    width: 100%;
    margin-bottom: 2rem;
  }
  &__txt {
    display: flex;
    flex-direction: column;
    justify-content: center;
    &-title {
      font-size: 2.6rem;
      margin: 4rem 0 2rem 0;
    }
    &-list {
      margin-top: 3rem;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 0 5%;
      list-style: none;
      font-size: 1.8rem;
      &-item {
        display: flex;
        &:not(:first-child) {
          margin-top: 3rem;
        }
        &-icon {
          height: 2rem;
        }
        & span {
          margin-left: 1rem;
          font-weight: 700;
        }
      }
    }
  }
}
</style>
