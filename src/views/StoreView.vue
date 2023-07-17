<template>
    <div class="about">
      <h1>This is an store page</h1>
      <ListProduct />
    </div>
  </template>
  
<script lang="ts">
import ListProduct from '@/components/ListProduct.vue';

export default{
  components: {
    ListProduct,
  },
}
</script>

