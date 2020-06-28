<template>
  <div>
    <b-navbar variant="transparent" type="dark">
      <b-navbar-brand to="/">
        {S}
      </b-navbar-brand>
      <b-navbar-nav class="ml-auto">
        <b-nav-item to="/">
          Inicio
        </b-nav-item>
        <b-nav-item to="/about">
          Sobre mi
        </b-nav-item>
        <b-nav-item to="/portfolio">
          Portafolio
        </b-nav-item>
      </b-navbar-nav>
    </b-navbar>
    <b-aspect aspect="16:9" tag="header" class="header">
      <b-container class="header__cover d-flex justify-content-center align-items-center text-light flex-column flex-sm-row" fluid>
        <b-img
          class="header__img border border-primary"
          src="../assets/img/sergio-azocar.jpg"
          height="130px"
          width="130px"
          rounded="circle"
          alt="Circle image"
        />
        <div class="ml-sm-4">
          <h1 class="header__title display-4">
            Sergio Azócar
          </h1>
          <p class="header__subtitle lead">
            Frontend Developer
          </p>
        </div>
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
  max-height: 65vh;
  background-image: url("../assets/img/fondo-header-sergioazoc.jpg");
  background-size: cover;
  background-position: 50% 32%;
}
.header__cover{
  $color: #007bff73;
  $body-bg: #250657;
  height: 100%;
  background: $color linear-gradient(0deg, $body-bg, $color) repeat-x;
}
@media (max-width: 575.98px){
  .header__img{
    margin-top: 30px;
    height: 100px;
    width: 100px;
  }
  .header__title{
    font-size: 2.5rem;
  }
  .header__subtitle{
    text-align: center;
  }
}
.footer{
  background-color: #250657;
  margin-top: 30px;
}
</style>
