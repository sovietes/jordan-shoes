<template>
  <section class="presentation">
    <div class="text-presentation">
      <vue-typed-js :type-speed="50" :strings="['A melhor loja de Jordan']">
        <p class="title typing"></p>
      </vue-typed-js>
      <vue-typed-js
        :contentType="'html'"
        :type-speed="50"
        :strings="[
          'O tênis Jordan é fruto de uma velha e<br> forte parceria entre a Nike e o jogador Michael Jordan.',
        ]"
      >
        <p class="description typing"></p>
      </vue-typed-js>
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
  background-attachment: fixed;
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
