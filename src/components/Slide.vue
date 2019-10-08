<template>
  <div class="slide">
    <div class="slide-content">
      <slot />
    </div>
  </div>
</template>

<script>
  export default {
    name: 'slide'
  }
</script>

<style lang="scss" scoped>
.slide {
  height: 100vh;
  background: #f31912;
  color: #fff;
  font-weight: bold;
  font-size: 5rem;
  padding: 3rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  &-content {
    max-width: 1200px;
  }
}
</style>