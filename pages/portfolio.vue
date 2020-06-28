<template>
  <b-container fluid="sm" tag="section">
    <h2>Portafolio 👨‍💻</h2>
    <p class="lead">
      Estos son algunos proyectos que he realizado, sea por trabajo o sólo por hobby con la intención de aprender algo nuevo.
    </p>
    <b-row cols="1" cols-sm="2" cols-md="3">
      <b-col v-for="(proyecto, index) in proyectos" :key="index" class="mb-3">
        <div class="card h-100">
          <div class="card-body">
            <p class="card-title h4">
              {{ proyecto.title }}
            </p>
            <p class="card-text">
              {{ proyecto.description }}
            </p>
            <div class="mb-3">
              <span v-for="(tag, i) in proyecto.tags" :key="i" class="badge py-1 badge-primary badge-pill mr-1">
                {{ tag.name }}
              </span>
            </div>
            <a :href="proyecto.url" class="btn btn-outline-primary btn-sm">ir al proyecto</a>
          </div>
        </div>
      </b-col>
    </b-row>
  </b-container>
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
