<script setup lang="ts">
import { RouterView } from 'vue-router';
import HeaderComponent from '@/components/HeaderComponent.vue';
</script>

<template>
  <div class="app-container">
    <header>
      <HeaderComponent />
    </header>
    <main class="main">
      <RouterView />
    </main>
    <footer>
      <span>footer</span>
    </footer>
  </div>
</template>

<style lang="scss">
@import '@/assets/base.scss';
</style>
