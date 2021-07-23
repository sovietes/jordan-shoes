<template>
  <footer>
    <p>Todos os direitos reservados.</p>
  </footer>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({})
</script>
<style scoped>
footer {
  background: var(--dark-color);
  margin-top: 100px;
  height: 60px;
  display: flex;
  justify-content: center;
  align-items: center;
}

p {
    font-weight: 500;
    font-size: 1.125rem;
    color: #F6F6F6;
    margin: 1rem;
}
</style>
