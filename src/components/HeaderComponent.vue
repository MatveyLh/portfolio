<script setup lang="ts">
import FilledLinkComponent from '@/components/link/FilledLinkComponent.vue';
import LinkComponent from './link/LinkComponent.vue';
</script>

<template>
  <div class="container">
      <LinkComponent href="/" label="Home" />
      <div class="right">
        <div class="rightItem">
          <LinkComponent href="/projects" label="Projects" />
        </div>
        <div class="rightItem">
          <FilledLinkComponent href="/contact" label="Contact" variant="filled" />
        </div>
      </div>
  </div>
</template>

<style scoped lang="scss">
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 40px 0;
  }

  .right {
    display: flex;
  }

  .rightItem {
    display: flex;
    align-items: center;
    margin-left: 87px;

    &:first-child {
      margin-left: 0;
    }
  }
</style>
