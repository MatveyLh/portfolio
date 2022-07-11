<script setup lang="ts">
import { RouterLink } from 'vue-router';

defineProps<{
  href: string,
  label: string,
}>();
</script>

<template>
  <RouterLink class="defaultLinkStyle" :to="href">{{ label }}</RouterLink>
</template>

<style scoped lang="scss">
  @import '@/assets/colors.scss';
  @import './coreStyle.scss';
</style>
