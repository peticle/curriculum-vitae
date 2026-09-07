<script setup lang="ts"></script>

<template>
  <li class="dot-list-item">
    <span class="dot-list-item_dot"></span>
    <div>
      <span class="dot-list-item_left" v-if="$slots.left">
        <slot name="left" />
      </span>
      <span class="dot-list-item_right">
        <slot name="right" />
      </span>
    </div>
  </li>
</template>

<style lang="scss" scoped>
.dot-list-item {
  display: flex;
  gap: 1rem;

  &_dot {
    background: var(--theme-clr-primary);
    border-radius: 50%;
    flex-shrink: 0;
    height: 0.4em;
    margin: 0.5em 0 0;
    width: 0.4em;
  }

  div {
    display: flex;
    flex-grow: 1;
    gap: 0.6rem;
  }

  &_left:deep(svg) {
    margin: 0.1em 0 0;
  }

  &_right {
    flex-grow: 1;
  }
}
</style>
