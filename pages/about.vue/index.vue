<template>
  <section class="about">
    <img src="~/assets/img/about/feet-splash.jpg" class="about__img" />
    <h1 class="about__title">About</h1>
    <p class="about__txt">
      Global Orthotics Inc. is a Canadian Orthotic Lab that offers a wide
      variety of Innovative Custom Made Orthotics. We have a highly medical team
      of Podiatrist, Chiropodist, and Pedorthist that help design the best and
      most innovative orthotic devices.
    </p>
    <p class="about__txt">
      At Global Orthotics Inc. we strive for the best quality along with the
      greatest customer service. Our entire line of Custom Made Orthotics are
      handcrafted from start to finish by our team of skilled technicians.
      Global Orthotic Team never stop researching on best material that make a
      better orthotic device. Our modern technology and handcraft make us an
      exquisite team.
    </p>
  </section>
</template>

<style lang="scss">
.about {
  margin-top: 10rem;
  padding-bottom: 5rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  &__img {
    width: 100%;
    height: 15rem;
    object-fit: cover;
  }
  &__title {
    font-size: 3.3rem;
    margin-top: 4rem;
  }
  &__txt {
    margin-top: 3rem;
    padding: 0 5%;
    line-height: 3rem;
    font-size: 1.6rem;
  }
}
</style>
