<template>
  <div id="app">
    <carousel :items="1" :autoplay="true" :nav="false" class="carousel">
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
      <slide>
        <p>¿Los poderosos?</p>
        <p>No, a esos no les hace falta un gobierno. De hecho, les molesta que alguien les controle.</p>
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
}

.delayed {
  animation: reveal;
}
</style>
