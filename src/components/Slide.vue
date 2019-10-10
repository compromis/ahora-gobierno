<template>
  <div class="slide" :style="{ backgroundColor: color }">
    <div class="slide-content">
      <slot />
    </div>
  </div>
</template>

<script>
  export default {
    name: 'slide',

    props: {
      color: String
    }
  }
</script>

<style lang="scss" scoped>
.slide {
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
    max-width: 1200px;
  }
}

.smaller {
  font-size: calc(1.5rem + 1.5vw);
}

.delayed {
  opacity: 0;
  animation-name: reveal;
  animation-duration: 1s;
  animation-delay: .5s;
  animation-fill-mode: forwards;
}

@keyframes reveal {
  from { opacity: 0; }
  to { opacity: 1; }
}
</style>