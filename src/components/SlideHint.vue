<template>
  <div>
    <svg version="1.1" x="0px" y="0px" width="18px" height="19px" viewBox="0 0 18 19" style="enable-background:new 0 0 18 19;" xml:space="preserve">
    <defs>
    </defs>
    <g>
      <path class="chevron-1" fill="#fff" d="M0.15,0.85c-0.2-0.2-0.2-0.51,0-0.71c0.2-0.2,0.51-0.2,0.71,0l9,9c0.2,0.2,0.2,0.51,0,0.71l-9,9c-0.2,0.2-0.51,0.2-0.71,0
        c-0.2-0.2-0.2-0.51,0-0.71L8.79,9.5L0.15,0.85z"/>
      <path class="chevron-2" fill="#fff" d="M16.79,9.5L8.15,0.85c-0.2-0.2-0.2-0.51,0-0.71c0.2-0.2,0.51-0.2,0.71,0l9,9c0.2,0.2,0.2,0.51,0,0.71l-9,9
        c-0.2,0.2-0.51,0.2-0.71,0c-0.2-0.2-0.2-0.51,0-0.71L16.79,9.5z"/>
    </g>
    </svg>
  </div>
</template>

<script>
  export default {
    name: 'slide-hint'
  }
</script>

<style lang="scss" scoped>
.chevron-1 {
  animation: chevron 1.2s ease-in-out 0s infinite;
}
.chevron-2 {
  animation: chevron 1.2s ease-in-out 0.8s infinite;
}

@keyframes chevron {
  0% {
    opacity: 0.4;
  }
  33% {
    opacity: 1;
  }
  66% {
    opacity: 0.4;
  }
  100% {
    opacity: 0.4;
  }
}

</style>

