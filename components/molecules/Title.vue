<template>
  <section class="title">
    <p class="title-des">Destaques</p>
    <p class="description">
      Frete grátis e chinelo de brinde é aqui, aproveite por tempo limitado.
    </p>
  </section>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({})
</script>
<style scoped>
.title {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  margin-top: 3.625rem;
}

.title-des {
  font-size: 2rem;
  font-weight: 600;
  line-height: 62.78px;
}

.description {
  font-weight: 500;
  font-size: 1rem;
  line-height: 31.39px;
  text-align: center;
  margin: 0 1rem 4rem 1rem;
}
</style>
