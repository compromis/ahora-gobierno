<template>
  <div class="slide" :style="{ backgroundColor: color }">
    <div class="slide-content">
      <slot />
    </div>
    <div v-if="background" class="slide-background" :style="{ backgroundImage:  `url(${background})` }"></div>
  </div>
</template>

<script>
  export default {
    name: 'slide',

    props: {
      color: String,
      background: String
    }
  }
</script>

<style lang="scss" scoped>
.slide {
  position: relative;
  height: 100vh;
  background: #f31912;
  color: #fff;
  font-weight: bold;
  font-size: calc(2rem + 2vw);
  padding: 3rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  line-height: 1.25;

  &-content {
    position: relative;
    max-width: 1200px;
    z-index: 10;
  }

  &-background {
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    filter: grayscale(100%);
    z-index: 0;
    opacity: .45;
    background-size: cover;
    background-position: center;
  }

  h3 {
    font-size: calc(1rem + .25vw);
    border: 3px #fff solid;
    padding: 1rem 2rem;
    letter-spacing: 1px;
    max-width: 800px;
    margin: 0 auto;
  }

  .smaller {
    font-size: calc(1.25rem + 1.25vw);
  }

  .delayed {
    opacity: 0;
    animation-name: reveal;
    animation-duration: 1s;
    animation-delay: 1s;
    animation-fill-mode: forwards;
  }
}

@keyframes reveal {
  from { opacity: 0; }
  to { opacity: 1; }
}
</style>