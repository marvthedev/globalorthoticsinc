<!--
  globalorthoticsinc by Marvin Marinas 
  https://www.marvinmarinas.com
  Website and graphics design.
-->
<template>
  <div>
    <topNav />
    <Nuxt />
    <foot />
  </div>
</template>

<script>
import topNav from '~/components/TopNav'
import foot from '~/components/Foot'

export default {
  components: {
    topNav,
    foot
  }
}
</script>

<style>
html {
  font-family: 'Open Sans', sans-serif;
  font-size: 62.5%;
  font-weight: 300;
  color: #777777;
  word-spacing: 0;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  border: none;
}

/* Typography Defaults */
h1,
h2 {
  color: #212529;
}

h1 {
  font-weight: 700;
}

p {
  font-size: 1.8rem;
  line-height: 3rem;
}

a {
  text-decoration: none;
  color: inherit;
}

/* Forms */
input,
textarea {
  font-family: inherit;
  font-size: 1.4rem;

  /* Remove unwanted thick border-top on iOS devices */
  -webkit-appearance: none;
}

textarea {
  resize: none;
}
</style>
