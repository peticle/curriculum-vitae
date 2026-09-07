<script setup lang="ts">
import picture from "@/assets/picture.png";
</script>

<template>
  <header>
    <h1 class="hidden">Curriculum vitæ de Clément Petignat</h1>
    <img :src="picture" alt="Une photo de moi" />
    <div>
      <span></span>
      <div class="flex-col">
        <strong>Clément PETIGNAT</strong>
        <span>Ingénieur en informatique HES</span>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
header {
  align-items: center;
  background: url("/header.png");
  color: var(--theme-clr-light);
  display: grid;
  grid-template-columns: 2fr 3fr;

  img {
    align-self: flex-end;
    filter: grayscale(1);
    justify-self: center;
    margin: 0.6rem 0 0;
    max-width: 100px;
  }

  > div {
    display: flex;
    flex-wrap: wrap;
    gap: 0.6rem;
    padding: 0 1.4rem;

    > span {
      background: white;
      border-radius: 0.2em;
      display: block;
      flex-shrink: 0;
      min-height: 100%;
      width: 0.4em;
    }

    > div {
      font-size: 1.6em;
      gap: 0.4rem;
      padding: 0.2em;

      span {
        font-size: 0.8em;
      }
    }
  }
}
</style>
