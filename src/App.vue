<template>
  <Product :price="1500" :name="product" available />
</template>

<script setup lang="ts">
import { ref } from 'vue';
import Product from './Product.vue';

const product = ref('Voiture');
</script>

<style scoped lang="scss"></style>
