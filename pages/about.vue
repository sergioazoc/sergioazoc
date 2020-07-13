<template>
  <div>
    <b-container fluid="sm" tag="section">
      <h2>Sobre mi</h2>
      <p class="lead">
        Actualmente estoy enfocado en el desarrollo frontend, trabajando con vue/react  y javascript en general. Tengo buen dominio de HTML/CSS y algunos frameworks de css como bootstrap o materialize.
      </p>
      <p class="lead">
        Entre 2016 y el 2019 emprendí con una agencia y una academia digital, dónde aprendí bastante sobre branding y marketing en general (SEO, social media, inbound, etc.), esto gracias a los muchos cursos que hice (<a href="https://platzi.com/@sergioazocar/" target="_blank" rel="noopener noreferrer">Platzi</a>) y el trabajo con clientes. Durante ese tiempo implementé diversos sitios web con wordpress y tiendas con woocommerce, además de algunos desarrollos con PHP, Ruby on Rails, HTML/CSS.
      </p>
      <p class="lead">
        Así como me gusta aprender, también enseñar, lo que me llevó a realizar charlas, seminarios, cursos y mentorías en varias ciudades del sur de Chile.
      </p>
    </b-container>
    <b-container fluid="sm" tag="section">
      <h2 class="mb-2">
        Estudios
      </h2>
      <ul>
        <li class="lead">
          Analista Programador (Inacap)
        </li>
        <li class="lead">
          Técnico de nivel medio en Electrónica (Liceo)
        </li>
        <li class="lead">
          Monitor de física experimental (USACH)
        </li>
      </ul>
    </b-container>
    <b-container fluid="sm" tag="section">
      <h2 class="mb-2">
        Cursos realizados
      </h2>
      <b-row cols="1" cols-sm="2" cols-md="3">
        <b-col v-for="(curso, index) in cursos" :key="index" class="d-flex align-items-center mb-4">
          <div class="course d-flex align-items-center">
            <img :src="curso.badge" class="course__badge mr-3" :alt="curso.title">
            <a :href="curso.diploma_link" target="_blank" rel="noopener noreferrer">
              <span class="lead">{{ curso.title }}</span>
            </a>
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import Courses from '../static/Courses.json'
export default {
  data () {
    return {
      cursos: []
    }
  },
  created () {
    this.cursos = Courses
  }
}
</script>

<style scoped>
.course a{
  color: #250657
}
.course a:hover{
  text-decoration: none;
  color: #6610f2;
}
.course__badge{
  width: 50px;
  height: 50px;
}
</style>
