<template>
  <div class="orthotics">
    <img src="~/assets/img/orthotics/feet-walk.jpg" class="orthotics__img" />
    <div class="orthotics__txt">
      <h2 class="orthotics__title">Orthotics: What are they?</h2>
      <p>
        Orthotics are customized footwear inserts that is prescribed by a
        doctor. It is specifically made for the individual to treat foot, leg or
        back problems.
      </p>
      <h2 class="orthotics__title">What Problems Can Orthotics Fix?</h2>
      <p>Orthotics can fix some of the following problems:</p>
    </div>
  </div>
</template>

<style lang="scss">
.orthotics {
  margin-top: 10rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  min-height: 90vh;
  width: 100%;
  padding: 0 5%;
  &__img {
    width: 100%;
  }
  &__title {
    font-size: 2.6rem;
    margin: 2rem 0;
  }
}
</style>
