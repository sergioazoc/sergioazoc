<template>
  <div>
    <b-aspect aspect="16:9" tag="header" class="header">
      <b-container class="header__cover d-flex justify-content-center text-center flex-column text-light" fluid>
        <h1 class="display-4">
          Sergio Azócar
        </h1>
        <p class="lead">
          Frontend Developer
        </p>
      </b-container>
    </b-aspect>
    <b-container fluid="sm" tag="section" class="mt-5">
      <h2>Sobre mi 🤔</h2>
      <p class="lead mt-3">
        Soy un apasionado por saber cómo funcionan las cosas, por eso estudie electrónica, programación y marketing, también tengo conocimientos de diseño, ui/ux y branding. En aprendizaje constante y con hambre de crear!.
      </p>
    </b-container>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
.header{
  min-height: 50vh;
  max-height: 72vh;
  background-image: url("../assets/img/fondo-header-sergioazoc.jpg");
  background-size: cover;
  background-position: 50% 38%;
}
.header__cover{
  $color: #007bff73;
  $body-bg: #250657;
  height: 100%;
  background: $color linear-gradient(0deg, $body-bg, $color) repeat-x;
}
</style>
