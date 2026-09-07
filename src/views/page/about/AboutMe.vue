<script setup lang="ts">
import { Calendar1, House, Mail, Phone, User } from "@lucide/vue";
import Github from "@/assets/github.svg?component";
import { DotList, DotListItem, SectionTitle } from "@/components";
</script>

<template>
  <section id="about_me">
    <SectionTitle>
      <template #icon><User /></template>
      <h3>À propos</h3>
    </SectionTitle>
    <DotList>
      <DotListItem>
        <template #left>
          <Calendar1 />
        </template>
        <template #right>
          <date>21 février 1999</date>
        </template>
      </DotListItem>
      <DotListItem>
        <template #left>
          <Mail />
        </template>
        <template #right>
          <a href="mailto:clement.petignat@protonmail.com"> clement.petignat@protonmail.com </a>
        </template>
      </DotListItem>
      <DotListItem>
        <template #left>
          <Phone />
        </template>
        <template #right>
          <a href="tel:+41798423403">079 842 34 03</a>
        </template>
      </DotListItem>
      <DotListItem>
        <template #left>
          <House />
        </template>
        <template #right>
          <span>2900 Porrentruy, JU</span>
        </template>
      </DotListItem>
      <DotListItem>
        <template #left>
          <Github class="github" />
        </template>
        <template #right>
          <a href="https://github.com/peticle">github.com/peticle</a>
        </template>
      </DotListItem>
    </DotList>
  </section>
</template>

<style lang="scss" scoped>
#about_me:deep(svg) {
  max-height: 1em;
  width: 1em;

  &.github {
    fill: var(--theme-clr-foreground);
  }
}
</style>
