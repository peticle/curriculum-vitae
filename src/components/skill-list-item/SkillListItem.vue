<script setup lang="ts"></script>

<template>
  <li class="skill-list-item">
    <span class="skill-list-item_left">
      <slot name="left" />
    </span>
    <span class="skill-list-item_right">
      <slot name="right" />
    </span>
  </li>
</template>

<style lang="scss" scoped>
.skill-list-item {
  align-items: center;
  display: grid;
  grid-template-columns: 3fr 1fr;
}
</style>
