<script setup lang="ts"></script>

<template>
  <ul class="skill-list">
    <li>
      <span>Domaine</span>
      <span>Maîtrise</span>
    </li>
    <slot />
  </ul>
</template>

<style lang="scss" scoped>
.skill-list {
  display: flex;
  flex-direction: column;

  li {
    display: grid;
    grid-template-columns: 3fr 1fr;

    &:first-of-type {
      font-size: 0.8em;
      font-weight: lighter;
    }

    span {
      font-style: italic;
    }
  }
}
</style>
