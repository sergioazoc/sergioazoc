<template>
  <div>
    <section class="container">
      <h2>En pocas palabras... 🤔</h2>
      <p class="lead mt-3">
        Soy un apasionado por saber cómo funcionan las cosas y un creador empedernido, por eso estudie electrónica, programación y marketing, también tengo conocimientos de diseño, ui/ux y branding. En aprendizaje constante y con hambre de hacer cosas nuevas!.
      </p>
    </section>
    <section class="container mt-5">
      <h2>Tecnologías y herramientas que he usado</h2>
      <div class="mt-3">
        <span v-for="(tecnologia, index) in tecnologias" :key="index" class="border border-primary badge text-primary">{{ tecnologia.name }}</span>
      </div>
    </section>
    <section class="container">
      <h2 class="mb-4">
        Comunidades en las que participo
      </h2>
      <div class="row">
        <div class="col-12 col-md-6 mb-3">
          <div class="card h-100">
            <img src="../assets/img/startupweekend.jpg" alt="Startup Weekend" class="card-img-top">
            <div class="card-body">
              <p class="card-text">
                Coorganizador de <a href="https://www.facebook.com/swloslagos" target="_blank" rel="noopener noreferrer">Startup Weekend Los Lagos</a>, dónde enseñamos a crear una startup en 54 horas.
              </p>
            </div>
          </div>
        </div>
        <div class="col-12 col-md-6 mb-3">
          <div class="card h-100">
            <img src="../assets/img/devs&ops.jpg" alt="Devs&Ops Los Lagos" class="card-img-top">
            <div class="card-body">
              <p class="card-text">
                Staff de la comunidad de <a href="https://www.facebook.com/devsopsLosLagos" target="_blank" rel="noopener noreferrer">Devs&Ops Los Lagos</a>, dónde organizamos eventos, meetups y networking para programadores de la región.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import Technologies from '../static/Technologies.json'
import ogImage from '../assets/img/og-sergioazoc.jpg'
export default {
  data () {
    return {
      tecnologias: []
    }
  },
  created () {
    this.tecnologias = Technologies
  },
  head () {
    return {
      meta: [
        { hid: 'og:image', name: 'og:image', content: ogImage }
      ]
    }
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
