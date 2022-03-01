<template>
  <h3>{{ title }} - {{ price }}€</h3>
</template>

<script setup lang="ts">
import { computed } from 'vue';
const props = defineProps({
  name: {
    type: String,
    required: true,
  },
  price: Number,
});
const title = computed(() => props.name.toUpperCase());
</script>

<style scoped lang="scss"></style>
