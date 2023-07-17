<template>
  <Navbar></Navbar>
  <RouterView />
</template>

<script lang="ts">
  import Navbar from '@/components/Navbar.vue';
  

  export default {
    components: 
    {
      Navbar,
    }
  }
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  background-color: whitesmoke;
}
</style>
