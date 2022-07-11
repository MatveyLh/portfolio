<script setup lang="ts">
import { RouterLink } from 'vue-router';

defineProps<{
  href: string,
  label: string,
}>();
</script>

<template>
  <RouterLink class="filledLinkStyle" :to="href">{{ label }}</RouterLink>
</template>

<style scoped lang="scss">
  @import '@/styles/colors.css';
  @import './coreStyle.scss';
</style>
