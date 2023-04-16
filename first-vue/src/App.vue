<!-- composition API -->
<!-- <script setup>
import { ref } from 'vue';

const count = ref(0)
</script> --> 

<!-- option API -->

<script>
export default ({
  data() {
    return {
      count: 0
    }
  },
  methods: {
    AddCount() {
      this.count += 1
    },
    SubtractCount(){
      this.count -= 1
    }
  }
})
</script>


<template>
  <main>
    <div>
      <h1>{{ count }}</h1>
      <button id="inc" @click="SubtractCount()">-</button>
      <button id="dec" @click="AddCount()">+</button>
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
