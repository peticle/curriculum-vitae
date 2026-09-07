<script setup lang="ts">
import {
  ExperienceLanguages,
  ExperienceProfessional,
  ExperienceSkills,
} from "@/views/page/experience";
</script>

<template>
  <section id="experiences">
    <h2 class="hidden">Expériences</h2>
    <ExperienceProfessional />
    <ExperienceSkills />
    <ExperienceLanguages />
  </section>
</template>
<style lang="scss" scoped>
#experiences {
  background: var(--theme-clr-light);
  gap: 0.8rem;
  justify-content: space-between;
  padding: 2em 1.4rem;
}
</style>
