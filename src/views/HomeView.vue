<template>
  <h1>HomePage</h1>
  <ListProduct/>
  
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import ListProduct from '@/components/ListProduct.vue';

@Options({
  components: {
    ListProduct,
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