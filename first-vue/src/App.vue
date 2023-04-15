<script setup>
import { ref } from 'vue';

const count = ref(0)
</script>

<template>
  <main>
    <div>
      <h1>{{ count }}</h1>
      <button id="inc" @click="count++">+</button>
      <button id="dec" @click="count--">-</button>
    </div>
  </main>
</template>

<style scoped>
main {

  height: 50vh;
  width: 50vw;
  background: rgba(8, 107, 194, 0.548);
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}
</style>