<script setup lang="ts">
import { RouterLink } from 'vue-router';

defineProps<{
  href: string,
  label: string,
}>();
</script>

<template>
  <RouterLink class="link" :to="href">{{ label }}</RouterLink>
</template>

<style scoped lang="scss">
@import '@/assets/colors.scss';

.link {
  display: block;
  font-size: 16px;
  line-height: 20px;
  text-decoration: none;
  transition: background-color 0.2s ease;
  color: $white;
  background-color: $primary;
  padding: 12px 20px;
  border-radius: 6px;

  &:hover {
    background-color: $primary__dark;
  }
}
</style>
