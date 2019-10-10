<template>
  <div id="app">
    <carousel :items="1" :autoplay="true" class="carousel">
      <slide>
        <p>¿Ahora, gobierno?</p>
        <p class="delayed">¿Y en los últimos 4 meses? ¿Por qué no?</p>
      </slide>
      <slide>
        <p>¿Quizás porque os han importado más las siglas que las personas?</p>
      </slide>
      <slide>
        <p>¿Sabéis quien está pagando vuestra irresponsabilidad?</p>
      </slide>
      <slide color="#000">
        <p>¿Los poderosos?</p>
        <p class="delayed smaller">No, a esos no les hace falta un gobierno. De hecho, les molesta que alguien les controle.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1461088945293-0c17689e48ac?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2702&q=80">
        <h3>LA IRRESPONSABILIDAD DE NO QUERER FORMAR UN GOBIERNO PROGRESISTA LA PAGAN:</h3>
        <p>Las personas</p>
        <p class="smaller">Porque se bloquean fondos para Educación, sanidad, dependencia o servicios sociales.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1512405228606-d71b7aa8d110?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1000&q=60">
        <h3>LA IRRESPONSABILIDAD DE NO QUERER FORMAR UN GOBIERNO PROGRESISTA LA PAGAN:</h3>
        <p>Los precarios</p>
        <p class="smaller">Porque no se deroga la reforma laboral ni se activa la lucha contra la explotación.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1438761681033-6461ffad8d80?ixlib=rb-1.2.1&auto=format&fit=crop&w=2700&q=80">
        <h3>LA IRRESPONSABILIDAD DE NO QUERER FORMAR UN GOBIERNO PROGRESISTA LA PAGAN:</h3>
        <p>Las mujeres</p>
        <p class="smaller">Porque no se aprueban más medidas contra la violencia machista.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1416169607655-0c2b3ce2e1cc?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1000&q=60">
        <h3>LA IRRESPONSABILIDAD DE NO QUERER FORMAR UN GOBIERNO PROGRESISTA LA PAGAN:</h3>
        <p>El medio ambiente</p>
        <p class="smaller">Porque no se aprueba una Ley de lucha contra la Emergencia Climática.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1506919258185-6078bba55d2a?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1715&q=80">
        <h3>LA IRRESPONSABILIDAD DE NO QUERER FORMAR UN GOBIERNO PROGRESISTA LA PAGAN:</h3>
        <p>Jóvenes</p>
        <p class="smaller">Porque no se aumentan las becas, ni se limita el precio del alquiler.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1524067217094-584e94e61106?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1000&q=60">
        <h3>LA IRRESPONSABILIDAD DE NO QUERER FORMAR UN GOBIERNO PROGRESISTA LA PAGAN:</h3>
        <p>Mayores</p>
        <p class="smaller">Porque no se garantizan unas pensiones dignas.</p>
      </slide>
      <slide color="orangered">
        <p>Para salir del bloqueo.</p>
        <p class="smaller">Para conseguir un gobierno que mejore la vida de las personas y no de los poderosos.</p>
        <p class="smaller">¡ÚNETE!</p>
        <div>FB...</div>
      </slide>
    </carousel>
  </div>
</template>

<script>
import carousel from 'vue-owl-carousel'
import Slide from './components/Slide'

export default {
  name: 'app',
  components: {
    Slide,
    carousel
  }
}
</script>

<style lang="scss">
* {
  box-sizing: border-box;
}
body {
  margin: 0;
}

#app {
  font-family: 'Poppins', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.carousel {
  position: relative;
}

.owl-dots {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  padding: 2rem;
}

.owl-theme {
  .owl-nav {
    position: absolute;
    right: 3rem;
    bottom: 3rem;

    .owl-prev {
    display: none !important;
    }

    .owl-next {
      background-image: url(./assets/arrow.svg);
      background-color: transparent;
      text-indent: -9999px;
      height: 8rem;
      width: 8rem;
      background-position: center;
      background-size: 80%;
      border: 3px transparent solid;
      border-radius: 50%;
      background-repeat: no-repeat;
      transition: .25s ease-in-out;

      &:hover {
        border-color: #fff;
        background-image: url(./assets/arrow.svg);
        background-color: transparent !important;
        background-position: center;
        background-size: 80%;
        background-repeat: no-repeat;
      }

      &:active,
      &:focus {
        background-color: rgba(255, 255, 255, .5) !important;
      }
    }
  }
}
</style>
