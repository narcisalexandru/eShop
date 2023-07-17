<template>
  <div class="container">
    <Product v-for="product in listProduct" :key="product.id" :product="product"/>
  </div>
</template>

<script lang="ts">
import Product from '@/components/Product.vue';

export default {
  components: {
    Product,
  },
  data() {
    return {
      listProduct: [
        {
          id: 1,
          name: 'Bread',
          price: 2.5,
          image: require('@/assets/bread.png')
        },
        {
          id: 2,
          name: 'Water',
          price: 1.5,
          image: require('@/assets/water.png')
        },
        {
          id: 3,
          name: 'Apple',
          price: 1.99,
          image: require('@/assets/apple.png')
        },
        {
          id: 4,
          name: 'Banana',
          price: 0.99,
          image: require('@/assets//banana.png')
        },
        {
          id: 5,
          name: 'Orange',
          price: 1.49,
          image: require('@/assets/orange.png')
        },
        {
          id: 6,
          name: 'Strawberries',
          price: 3.99,
          image: require('@/assets/strawberries.png')
        },
        {
          id: 7,
          name: 'Pineapple',
          price: 2.99,
          image: require('@/assets/pineapple.png')
        },
        {
          id: 8,
          name: 'Watermelon',
          price: 4.99,
          image: require('@/assets/watermelon.png')
        },
        {
          id: 9,
          name: 'Grapes',
          price: 2.49,
          image: require('@/assets/grapes.png')
        },
        {
          id: 10,
          name: 'Pear',
          price: 1.79,
          image: require('@/assets/pear.png')
        },
        {
          id: 11,
          name: 'Cherry',
          price: 2.99,
          image: require('@/assets/cherry.png')
        },
        {
          id: 12,
          name: 'Mango',
          price: 3.49,
          image: require('@/assets/mango.png')
        }
      ]
    };
  },
}

</script>

<style scoped>
  .container {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    padding: 50px;
    gap: 50px;
  }
</style>
