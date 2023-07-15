<template>
   <BestProducts></BestProducts>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

import Navbar from '@/components/Navbar.vue'
import BestProducts from '@/components/BestProducts.vue';
import Product from '@/components/Product.vue';

@Options({
  components: {
    Navbar,
  },
})
export default class HomeView extends Vue {}
</script>


<style scoped>
  h1 {
    display: flex;
    align-items: center;
    align-content: center;
    justify-content: center;
  }
</style>