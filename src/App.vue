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
