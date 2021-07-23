<template>
  <section class="presentation">
    <div class="text-presentation">
      <p class="title">A melhor loja de Jordan</p>
      <p class="description">
        O tênis Jordan é fruto de uma velha e forte<br />parceria entre a Nike e
        o jogador Michael Jordan.
      </p>
    </div>
  </section>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({})
</script>
<style scoped>
img {
  display: block;
  max-width: 100%;
}

.presentation {
  height: 23.56rem;
  position: relative;
}

.presentation::before {
  content: '';
  background-image: url('@/assets/img/wallpaper.jpeg');
  height: 100%;
  position: absolute;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  filter: brightness(50%);
  width: 100%;
  z-index: -1;
}

.text-presentation {
  max-width: 1440px;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100%;
  gap: 1.1875rem;
}

.title {
  font-weight: 700;
  color: #f6f6f6;
  font-size: 2rem;
  margin: 0 1rem;
}

.description {
  font-weight: 500;
  font-size: 1.125rem;
  color: #f6f6f6;
  line-height: 20.31px;
  margin: 0 1rem;
}
</style>
