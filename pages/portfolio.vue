<template>
  <section class="container">
    <h2>Portafolio 👨‍💻</h2>
    <p class="lead">
      Estos son algunos proyectos que he realizado, sea por trabajo o sólo por hobby con la intención de aprender algo nuevo.
    </p>
    <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3">
      <div v-for="(proyecto, index) in proyectos" :key="index" class="col mb-3">
        <div class="card h-100">
          <div class="card-body">
            <p class="card-title h4">
              {{ proyecto.title }}
            </p>
            <p class="card-text">
              {{ proyecto.description }}
            </p>
            <div class="mb-3">
              <span v-for="(tag, i) in proyecto.tags" :key="i" class="badge rounded-pill bg-primary me-1 py-1">
                {{ tag.name }}
              </span>
            </div>
            <a :href="proyecto.url" class="btn btn-outline-primary btn-sm">ir al proyecto</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Projects from '../static/Projects.json'
export default {
  data () {
    return {
      proyectos: []
    }
  },
  created () {
    this.proyectos = Projects
  }
}
</script>
