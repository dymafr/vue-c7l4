<template>
  <h3>{{ title }} - {{ price }}€</h3>
</template>

<script setup lang="ts">
import { computed } from 'vue';
const props = defineProps({
  name: {
    type: String,
    required: true,
    validator(value: string): boolean {
      return value.length > 10;
    },
  },
  price: Number,
});
const title = computed(() => props.name.toUpperCase());
</script>

<style scoped lang="scss"></style>
