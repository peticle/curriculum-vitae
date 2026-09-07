<script setup lang="ts">
import { Languages } from "@lucide/vue";
import { DotList, DotListItem, SectionTitle } from "@/components";
</script>

<template>
  <section id="experience_languages">
    <SectionTitle>
      <template #icon><Languages /></template>
      <h3>Compétences linguistiques</h3>
    </SectionTitle>
    <DotList>
      <DotListItem>
        <template #right>
          <strong>Français : </strong>
          <span>langue maternelle</span>
        </template>
      </DotListItem>
      <DotListItem>
        <template #right>
          <strong>Anglais : </strong>
          <span> lu, écrit et parlé (niveau B2 &ndash; First Certificate) </span>
        </template>
      </DotListItem>
      <DotListItem>
        <template #right>
          <strong>Allemand : </strong>
          <span>notions</span>
        </template>
      </DotListItem>
    </DotList>
  </section>
</template>
