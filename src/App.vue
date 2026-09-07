<script setup lang="ts">
import { PageView } from "@/views";
import { FooterLayout, HeaderLayout } from "@/views/layout";
</script>

<template>
  <HeaderLayout />
  <main>
    <PageView />
  </main>
  <FooterLayout />
</template>

<style lang="scss" scoped>
main {
  display: grid;
  grid-template-columns: 2fr 3fr;
}
</style>
