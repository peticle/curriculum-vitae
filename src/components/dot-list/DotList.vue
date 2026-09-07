<script setup lang="ts"></script>

<template>
  <div class="dot-list">
    <span class="dot-list_bar"></span>
    <ul class="flex-col">
      <slot />
    </ul>
  </div>
</template>

<style lang="scss" scoped>
.dot-list {
  display: flex;
  position: relative;

  &_bar {
    background: var(--theme-clr-white);
    border-radius: 0.2em;
    display: block;
    height: 100%;
    left: 0.1em;
    position: absolute;
    top: 0;
    width: 0.2em;
  }

  ul {
    gap: 0.4rem;
    padding: 0.4em 0;
    z-index: 1;
  }
}
</style>
