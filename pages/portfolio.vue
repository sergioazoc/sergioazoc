<template>
  <b-container fluid="sm" tag="section">
    <h2>Portafolio 👨‍💻</h2>
    <p class="lead">
      Estos son algunos proyectos que he realizado, sea por trabajo o sólo por hobby con la intención de aprender algo nuevo.
    </p>
    <b-row cols="1" cols-sm="2" cols-md="3">
      <b-col class="mb-3">
        <b-card title="static-api-hots" class="h-100">
          <b-card-text>
            Api estática sobre el juego Heroes of the Storm, en español e inglés.
          </b-card-text>
          <b-card-text>
            <b-badge pill variant="primary" class="py-1">
              json
            </b-badge>
            <b-badge pill variant="primary" class="py-1">
              github pages
            </b-badge>
          </b-card-text>
          <b-button size="sm" href="https://sergioazoc.github.io/static-api-hots" target="_blank" variant="outline-primary">
            ir al proyecto
          </b-button>
        </b-card>
      </b-col>
      <b-col class="mb-3">
        <b-card title="pokedex-vue" class="h-100">
          <b-card-text>
            Buscador de pokémon basado en el api de PokeApi.
          </b-card-text>
          <b-card-text>
            <b-badge pill variant="primary" class="py-1">
              vue.js
            </b-badge>
            <b-badge pill variant="primary" class="py-1">
              vuex
            </b-badge>
            <b-badge pill variant="primary" class="py-1">
              vue-router
            </b-badge>
            <b-badge pill variant="primary" class="py-1">
              axios
            </b-badge>
          </b-card-text>
          <b-button size="sm" href="https://pokedex-vue.now.sh" target="_blank" variant="outline-primary">
            ir al proyecto
          </b-button>
        </b-card>
      </b-col>
      <b-col class="mb-3">
        <b-card title="covid_chile" class="h-100">
          <b-card-text>
            Muestra de datos oficiales de COVID en Chile, usando el api de chile-coronapi.
          </b-card-text>
          <b-card-text>
            <b-badge pill variant="primary" class="py-1">
              vue.js
            </b-badge>
            <b-badge pill variant="primary" class="py-1">
              vuex
            </b-badge>
            <b-badge pill variant="primary" class="py-1">
              vue-router
            </b-badge>
            <b-badge pill variant="primary" class="py-1">
              axios
            </b-badge>
          </b-card-text>
          <b-button size="sm" href="https://covid-chile.now.sh" target="_blank" variant="outline-primary">
            ir al proyecto
          </b-button>
        </b-card>
      </b-col>
      <b-col class="mb-3">
        <b-card title="cosmética kalu" class="h-100">
          <b-card-text>
            Sitio web para Kalu, marca de productos cosméticos con aceite de rosa mosqueta.
          </b-card-text>
          <b-card-text>
            <b-badge pill variant="primary" class="py-1">
              wordpress
            </b-badge>
            <b-badge pill variant="primary" class="py-1">
              woocommerce
            </b-badge>
          </b-card-text>
          <b-button size="sm" href="https://www.cosmeticakalu.cl/" target="_blank" variant="outline-primary">
            ir al proyecto
          </b-button>
        </b-card>
      </b-col>
      <b-col class="mb-3">
        <b-card title="hotel veliche" class="h-100">
          <b-card-text>
            Sitio web para Veliche, hotel y restaurant de Castro, Chiloé.
          </b-card-text>
          <b-card-text>
            <b-badge pill variant="primary" class="py-1">
              wordpress
            </b-badge>
            <b-badge pill variant="primary" class="py-1">
              2 idiomas
            </b-badge>
          </b-card-text>
          <b-button size="sm" href="https://www.veliche.cl/" target="_blank" variant="outline-primary">
            ir al proyecto
          </b-button>
        </b-card>
      </b-col>
    </b-row>
  </b-container>
</template>
