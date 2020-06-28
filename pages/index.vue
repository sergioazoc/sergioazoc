<template>
  <div>
    <b-container fluid="sm" tag="section">
      <h2>En pocas palabras... 🤔</h2>
      <p class="lead mt-3">
        Soy un apasionado por saber cómo funcionan las cosas, por eso estudie electrónica, programación y marketing, también tengo conocimientos de diseño, ui/ux y branding. En aprendizaje constante y con hambre de crear!.
      </p>
      <p class="lead">
        Coorganizador de <a href="https://www.facebook.com/swloslagos" target="_blank" rel="noopener noreferrer">Startup Weekend Los Lagos</a>, dónde enseñamos a crear una startup en 54 horas.
      </p>
      <p class="lead">
        Staff de la comunidad de <a href="https://www.facebook.com/devsopsLosLagos" target="_blank" rel="noopener noreferrer">Devs&Ops Los Lagos</a>, dónde organizamos eventos, meetups y networking para programadores de la región.
      </p>
      <p class="lead">
        Mentor en la red de Mentores de Impacto, dónde ayudo a emprendedores sobre temas digitales.
      </p>
    </b-container>
    <b-container tag="section" class="mt-5">
      <h2>Tecnologías que he usado</h2>
      <div class="mt-3">
        <span v-for="(tecnologia, index) in tecnologias" :key="index" class="border border-primary badge text-primary">{{ tecnologia.name }}</span>
      </div>
    </b-container>
  </div>
</template>

<script>
import Technologies from '../static/Technologies.json'
export default {
  data () {
    return {
      tecnologias: []
    }
  },
  created () {
    this.tecnologias = Technologies
  }
}
</script>

<style scoped>
.badge{
  font-size: 1rem;
  padding: 5px 10px;
  margin-right: 10px;
  margin-bottom: 10px;
}
</style>
