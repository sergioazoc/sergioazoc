<template>
  <div>
    <section class="container">
      <h2>Sobre mi</h2>
      <p class="lead">
        Este 2020 me volví a enamorar de la programación y estoy a full aprendiendo cosas nuevas y desarrollando proyectos en paralelo a mi trabajo como dev.
      </p>
      <p class="lead">
        Entre 2016 y el 2019 emprendí con una agencia y una academia digital, dónde aprendí bastante sobre branding y marketing en general (SEO, social media, inbound, etc.), esto gracias a los muchos cursos que hice (Platzi) y el trabajo con clientes. Durante ese tiempo implementé diversos sitios web ecommerce y corporativos, además de algunos desarrollos con PHP, Ruby on Rails, Javascript (vue/react), WordPress.
      </p>
      <p class="lead">
        Así como me gusta aprender, también enseñar, lo que me llevó a realizar charlas, seminarios, cursos y mentorías en varias ciudades del sur de Chile.
      </p>
    </section>
    <section class="container">
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
      <p>Actualmente realizando un curso de React/Hooks.</p>
    </section>
    <section class="container">
      <h2 class="mb-2">
        Cursos realizados
      </h2>
      <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3">
        <div v-for="(curso, index) in cursos" :key="index" class="col d-flex align-items-center mb-4">
          <div class="course d-flex align-items-center">
            <img :src="curso.badge" class="course__badge me-3" :alt="curso.title">
            <a :href="curso.diploma_link" target="_blank" rel="noopener noreferrer">
              <span class="lead">{{ curso.title }}</span>
            </a>
          </div>
        </div>
      </div>
    </section>
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
  color: #250657;
  text-decoration: none;
}
.course a:hover{
  color: #6610f2;
}
.course__badge{
  width: 50px;
  height: 50px;
}
</style>
