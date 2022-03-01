<template>
  <h3>{{ title }} - {{ price }}€</h3>
</template>

<script setup lang="ts">
import { computed } from 'vue';
import ProductI from './interfaces/product.interface.ts';

const props = defineProps<{product: ProductI}>());
const title = computed(() => props.name.toUpperCase());
</script>

<style scoped lang="scss"></style>
