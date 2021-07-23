<template>
  <section class="products">
    <div class="container">
      <div v-for="product in products" :key="product.id" class="item">
        <img :src="getLocale(product)">
      </div>
    </div>
  </section>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data() {
    return {
      products: [
        {
          id: 1,
          origin: '1.png',
        },
        {
          id: 2,
          origin: '2.png',
        },
        {
          id: 3,
          origin: '3.png',
        },
        {
          id: 4,
          origin: '4.png',
        },
        {
          id: 5,
          origin: '5.png',
        },
        {
          id: 6,
          origin: '6.png',
        },
        {
          id: 7,
          origin: '7.png',
        },
        {
          id: 8,
          origin: '8.png',
        },
      ],
    }
  },

  methods: {
    getLocale(item: any) {
      return require(`@/assets/img/${item.origin}`)
    }
  },
})
</script>
<style scoped>
.container {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem 1rem;
    margin: 0 1rem;
}

.item {
    background: var(--gray-color);
    width: 300px;
    height: 302px;
    display: flex;
    justify-content: center;
    align-items: center;
    justify-self: center;
}

img {
    display: block;
    max-width: 90%;
    width: 100%;
    margin-left: -5px;
}

.products {
    max-width: 1300px;
    margin: 0 auto;
}

@media screen and (max-width: 1300px) {
    .container {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }

    .products {
        max-width: 700px;
    }
}
</style>
