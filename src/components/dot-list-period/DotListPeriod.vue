<script setup lang="ts">
import { DotListItem } from "@/components";
</script>

<template>
  <DotListItem class="list-item">
    <template #right>
      <div class="flex-col">
        <strong><slot name="title" /></strong>
        <span v-if="$slots.subtitle" class="list-item_subtitle">
          <slot name="subtitle" />
        </span>
      </div>
      <span v-if="$slots.period" class="list-item_period">
        <slot name="period" />
      </span>
      <p v-if="$slots.description"><slot name="description" /></p>
    </template>
  </DotListItem>
</template>

<style lang="scss" scoped>
.list-item:deep(.dot-list-item_right) {
  display: flex;
  flex-wrap: wrap;
  gap: 0.2rem;
  justify-content: space-between;

  div {
    flex: 1 1 75%;
    gap: 0.2rem;
  }

  .list-item_period {
    font-weight: lighter;
    text-align: right;
  }

  p {
    font-size: 0.9em;
    font-style: italic;
    font-weight: lighter;
    text-align: justify;
    margin: 0;
    width: 100%;

    strong {
      font-weight: 500;
    }
  }
}
</style>
