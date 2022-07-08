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
    color: $black;
    font-weight: 500;
    font-size: 16px;
    line-height: 20px;
    transition: color 0.2s ease;
    text-decoration: none;

    &:hover {
      color: $primary;
    }
  }
</style>
