<template>
  <b-aspect aspect="16:9" tag="header" class="header">
    <b-container class="header__cover d-flex justify-content-center text-center flex-column text-light" fluid>
      <h1>
        Sergio Azócar
      </h1>
      <p>Frontend Developer</p>
    </b-container>
  </b-aspect>
</template>

<script>
export default {}
</script>

<style lang="scss">
.header{
  min-height: 50vh;
  max-height: 80vh;
  background-image: url("../assets/img/fondo-header-sergioazoc.jpg");
  background-size: cover;
  background-position: center;
}
.header__cover{
  $color: #6610f25e;
  $body-bg: #250657;
  height: 100%;
  background: $color linear-gradient(0deg, $body-bg, $color) repeat-x;
}
</style>
