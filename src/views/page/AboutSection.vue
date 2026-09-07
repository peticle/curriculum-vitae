<script setup lang="ts">
import { AboutInterests, AboutMe, AboutStudies } from "@/views/page/about";
</script>

<template>
  <section id="about" class="flex-col">
    <h2 class="hidden">A propos</h2>
    <AboutMe />
    <AboutStudies />
    <AboutInterests />
  </section>
</template>

<style lang="scss" scoped>
#about {
  background: var(--theme-clr-gray);
  color: var(--theme-clr-foreground);
  justify-content: space-between;
  padding: 2em 1.4rem;
}
</style>
