<template>
    <div class="about">
      <h1>This is an store page</h1>
    </div>
  </template>
  
  <script lang="ts">
import { Options, Vue } from 'vue-class-component';

import Navbar from '@/components/Navbar.vue'

@Options({
  components: {
    Navbar,
  },
})
export default class StoreView extends Vue {}
</script>

