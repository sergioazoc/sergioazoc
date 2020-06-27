<template>
  <div>
    <b-navbar variant="transparent" type="dark">
      <b-navbar-brand href="#">
        {S}
      </b-navbar-brand>
      <b-navbar-nav class="ml-auto">
        <b-nav-item to="/">
          Inicio
        </b-nav-item>
        <b-nav-item to="/portfolio">
          Portafolio
        </b-nav-item>
      </b-navbar-nav>
    </b-navbar>
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
    <Nuxt />
    <footer class="footer text-center py-2">
      <span class="lead text-light">Made with ♥ and Nuxt</span>
    </footer>
  </div>
</template>

<style lang="scss">
.navbar{
  margin-bottom: -56px;
}
.header{
  min-height: 50vh;
  max-height: 72vh;
  background-image: url("../assets/img/fondo-header-sergioazoc.jpg");
  background-size: cover;
  background-position: 50% 38%;
  margin-bottom: 50px;
}
.header__cover{
  $color: #007bff73;
  $body-bg: #250657;
  height: 100%;
  background: $color linear-gradient(0deg, $body-bg, $color) repeat-x;
}
.footer{
  background-color: #250657;
  margin-top: 30px;
}
</style>
