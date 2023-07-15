<template>
    <h1>This is an cart page</h1>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

import Navbar from '@/components/Navbar.vue'

@Options({
  components: {
    Navbar,
  },
})
export default class CartView extends Vue {}
</script>
