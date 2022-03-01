<template>
  <Product :price="1500" :name="product" />
</template>

<script setup lang="ts">
import { ref } from 'vue';
import Product from './Product.vue';

const product = ref('moto');
</script>

<style scoped lang="scss"></style>
