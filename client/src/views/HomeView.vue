<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <main>
    <div class="container">
      <div class="card card_small"></div>
      <div class="card card_medium"></div>
      <div class="card card_small"></div>
      <div class="card card_medium"></div>
      <div class="card card_large"></div>
      <div class="card card_small"></div>
      <div class="card card_medium"></div>
      <div class="card card_large"></div>
      <div class="card card_large"></div>
      <div class="card card_small"></div>
      <div class="card card_small"></div>
      <div class="card card_medium"></div>
      <div class="card card_large"></div>
      <div class="card card_small"></div>
      <div class="card card_medium"></div>
      <div class="card card_large"></div>
      <div class="card card_medium"></div>
      <div class="card card_large"></div>
    </div>
  </main>
</template>

<style>
  :root {
    --card_width: 250px;
    --card_border_radius: 16px;
    --row_increment: 10px;
    --card_large: 45;
    --card_medium: 33;
    --card_small: 26;
  }
  body {
    margin: 0;
    padding: 0;
    background-color: rgb(88, 88, 88);
  }
  .container {
    margin: 0;
    padding: 0;
    width: 80vw;
    /* background-color: black; */
    position: absolute;
    left: 50%;
    transform: translateX(-50%);

    display: grid;
    grid-template-columns: repeat(auto-fill, var(--card_width));
    grid-auto-rows: var(--row_increment);
    justify-content: center;
  }
  .card {
    padding: 0;
    margin: 15px 10px;
    background-color: rgb(128, 132, 148);
    border-radius: var(--card_border_radius);
  }
  .card_small {
    grid-row-end: span var(--card_small);
  }
  .card_medium {
    grid-row-end: span var(--card_medium);
  }
  .card_large {
    grid-row-end: span var(--card_large);
  }
</style>