<script setup lang="ts">
import FilledLink from '@/components/link/FilledLink.vue';
import Link from './link/DefaultLink.vue';
</script>

<template>
  <div class="container">
      <Link href="/" label="Home" />
      <div class="right">
        <div class="rightItem">
          <Link href="/projects" label="Projects" />
        </div>
        <div class="rightItem">
          <FilledLink href="/contact" label="Contact" variant="filled" />
        </div>
      </div>
  </div>
</template>

<style scoped lang="scss">
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 27px 0;
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
