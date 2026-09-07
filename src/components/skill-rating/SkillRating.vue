<script setup lang="ts">
import { computed } from "vue";
import type { SkillRatingProps } from "./skill-rating";

// Props
const props = defineProps<SkillRatingProps>();

// Computed
const width = computed<string>(() => {
  return `${props.rating * 100}%`;
});
</script>

<template>
  <span class="skill-rating">
    <span class="skill-rating_bar"></span>
  </span>
</template>

<style lang="scss" scoped>
@use "sass:math";

.skill-rating {
  $height: 0.4em;

  border: solid 1px black;
  border-radius: math.div($height, 2);
  display: flex;
  height: $height;
  overflow: hidden;

  &_bar {
    background: black;
    width: v-bind(width);
  }
}
</style>
