<script setup lang="ts"></script>

<template>
  <div class="section-title">
    <span></span>
    <slot name="icon" />
    <slot />
  </div>
</template>

<style lang="scss" scoped>
.section-title {
  align-items: center;
  display: flex;
  font-size: 1em;
  font-weight: bold;
  gap: 0.4rem;
  text-transform: uppercase;

  span {
    background: var(--theme-clr-primary);
    border-radius: 0.2em;
    display: block;
    height: 100%;
    margin: 0 0.6rem 0 0;
    width: 0.4em;
  }

  svg {
    max-height: 1.2em;
  }
}
</style>
