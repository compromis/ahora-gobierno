<template>
  <div id="app">
    <carousel v-if="lang === 'val'" :items="1" :autoplay="false" class="carousel">
      <slide>
        <p>¿Ahora, gobierno?</p>
        <p class="delayed">I en els últims 4 mesos?<br />Per què no?</p>
        <slide-hint class="slide-hint" />
      </slide>
      <slide>
        <p>Potser perquè us han importat més les sigles que les persones?</p>
      </slide>
      <slide>
        <p>Sabeu qui està pagant la vostra irresponsabilitat?</p>
      </slide>
      <slide color="#000">
        <p>Els poderosos?</p>
        <p class="delayed smaller">No, a eixos no els fa falta un govern. De fet, els molesta que algu els controle.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1461088945293-0c17689e48ac?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2702&q=80">
        <h3>LA IRRESPONSABILITAT DE NO VOLER FORMAR UN GOVERN PROGRESISTA LA PAGUEN:</h3>
        <p>Les persones</p>
        <p class="smaller">Perquè es bloquen fons per a educació, sanitat, dependència o serveis socials.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1512405228606-d71b7aa8d110?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1000&q=60">
        <h3>LA IRRESPONSABILITAT DE NO VOLER FORMAR UN GOVERN PROGRESISTA LA PAGUEN:</h3>
        <p>La gent treballadora</p>
        <p class="smaller">Perquè no es deroga la reforma laboral ni s'activa la luita contra la precarietat.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1438761681033-6461ffad8d80?ixlib=rb-1.2.1&auto=format&fit=crop&w=2700&q=80">
        <h3>LA IRRESPONSABILITAT DE NO VOLER FORMAR UN GOVERN PROGRESISTA LA PAGUEN:</h3>
        <p>Les dones</p>
        <p class="smaller">Perquè no s'aproven més mesures contra la violència masclista.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1416169607655-0c2b3ce2e1cc?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1000&q=60">
        <h3>LA IRRESPONSABILITAT DE NO VOLER FORMAR UN GOVERN PROGRESISTA LA PAGA:</h3>
        <p>El medi ambient</p>
        <p class="smaller">Perquè no s'aprova una Llei de lluita contra l'Emergència Climàtica.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1506377872008-6645d9d29ef7?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2850&q=80">
        <h3>LA IRRESPONSABILITAT DE NO VOLER FORMAR UN GOVERN PROGRESISTA LA PAGUEN:</h3>
        <p>La gent jove</p>
        <p class="smaller">Perquè no es limita el preu del lloguer, ni s'augmenten les beques.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1524067217094-584e94e61106?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1000&q=60">
        <h3>LA IRRESPONSABILITAT DE NO VOLER FORMAR UN GOVERN PROGRESISTA LA PAGUEN:</h3>
        <p>La gent major</p>
        <p class="smaller">Perquè no es garanteixen unes pensions dignes.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1561982479-c36896dad276?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1268&q=80">
        <h3>LA IRRESPONSABILITAT DE NO VOLER FORMAR UN GOVERN PROGRESISTA LA PAGUEN:</h3>
        <p>Las persones LGTBI</p>
        <p class="smaller">Perquè segueix sense aprovar-se una Llei Integral LGTBI i una Llei Trans, seguint l'exemple de les lleis valencianes.</p>
      </slide>
      <slide color="#f7921e">
        <p>Per a eixir del bloqueig.</p>
        <p class="smaller">Per a aconseguir un govern que millore la vida de les persones i no dels poderosos.</p>
        <p class="smaller">Acordar, la política útil</p>
        <a href="https://compromis.net" target="_blank" class="logo"><logo /></a>
      </slide>
    </carousel>
    <carousel v-else :items="1" :autoplay="false" class="carousel">
      <slide>
        <p>¿Ahora, gobierno?</p>
        <p class="delayed">¿Y en los últimos 4 meses?<br />¿Por qué no?</p>
        <slide-hint class="slide-hint" />
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
        <p class="smaller">Porque se bloquean fondos para educación, sanidad, dependencia o servicios sociales.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1512405228606-d71b7aa8d110?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1000&q=60">
        <h3>LA IRRESPONSABILIDAD DE NO QUERER FORMAR UN GOBIERNO PROGRESISTA LA PAGAN:</h3>
        <p>La gente trabajadora</p>
        <p class="smaller">Porque no se deroga la reforma laboral ni se activa la lucha contra la precariedad.</p>
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
      <slide color="#000" background="https://images.unsplash.com/photo-1506377872008-6645d9d29ef7?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2850&q=80">
        <h3>LA IRRESPONSABILIDAD DE NO QUERER FORMAR UN GOBIERNO PROGRESISTA LA PAGAN:</h3>
        <p>Jóvenes</p>
        <p class="smaller">Porque no se se limita el precio del alquiler, ni se aumentan las becas.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1524067217094-584e94e61106?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1000&q=60">
        <h3>LA IRRESPONSABILIDAD DE NO QUERER FORMAR UN GOBIERNO PROGRESISTA LA PAGAN:</h3>
        <p>Mayores</p>
        <p class="smaller">Porque no se garantizan unas pensiones dignas.</p>
      </slide>
      <slide color="#000" background="https://images.unsplash.com/photo-1561982479-c36896dad276?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1268&q=80">
        <h3>LA IRRESPONSABILIDAD DE NO QUERER FORMAR UN GOBIERNO PROGRESISTA LA PAGAN:</h3>
        <p>Las personas LGTBI</p>
        <p class="smaller">Porque sigue sin aprobarse una Ley Integral LGTBI y una Ley Trans, siguiendo el ejemplo de las leyes valencianas.</p>
      </slide>
      <slide color="#f7921e">
        <p>Para salir del bloqueo.</p>
        <p class="smaller">Para conseguir un gobierno que mejore la vida de las personas y no de los poderosos.</p>
        <p class="smaller">Acordar, la política útil</p>
        <a href="https://compromis.net" target="_blank" class="logo"><logo /></a>
      </slide>
    </carousel>
  </div>
</template>

<script>
import carousel from 'vue-owl-carousel'
import Slide from './components/Slide'
import SlideHint from './components/SlideHint'
import Logo from './components/Logo'

export default {
  name: 'app',
  components: {
    Slide,
    Logo,
    carousel,
    SlideHint
  },
  data () {
    return {
      lang: 'val'
    }
  },
  mounted () {
    this.calcVh()
    window.addEventListener('resize', this.calcVh)
  },
  methods: {
    calcVh () {
      let vh = window.innerHeight * 0.01
      document.documentElement.style.setProperty('--vh', `${vh}px`)
    }
  }
}
</script>

<style lang="scss">
* {
  box-sizing: border-box;
}

html,
body {
  height: 100%;
  margin: 0;
  overflow: hidden;
}

#app {
  font-family: 'Poppins', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.owl-carousel {
  position: fixed;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  overflow: hidden;
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
      background: transparent url(./assets/arrow.svg) !important;
      text-indent: -9999px;
      height: 8rem;
      width: 8rem;
      background-position: center !important;
      background-size: 80% !important;
      border: 3px transparent solid;
      border-radius: 50% !important;
      background-repeat: no-repeat !important;
      transition: .25s ease-in-out;

      &:hover {
        border-color: #fff;
        background: transparent url(./assets/arrow.svg) !important;
        background-position: center !important;
        background-size: 80% !important;
        background-repeat: no-repeat !important;
      }

      &:active,
      &:focus {
        background-color: rgba(255, 255, 255, .5) !important;
      }
    }
  }
}

.logo {
  display: block;
  width: 100%;
  max-width: 500px;
  margin: 0 auto;

  svg {
    width: 100%;
    height: 100%;
  }
}

.slide-hint {
  display: none;
}

@media screen and (max-width: 600px) {
  .owl-nav {
    bottom: 6rem !important;
  }

  .owl-next {
    display: none !important;
  }

  .owl-dots {
    padding: 1.25rem;

    .owl-dot {
      span {
        margin: 3px !important;
      }
    }
  }

  .slide-hint {
    display: block;
    position: fixed;
    bottom: 6rem;
    width: 100%;
    left: 0;
    right: 0;
    text-align: center;

    svg {
    width: 3.5rem;
    height: 3.5rem;
    }
  }
}
</style>
