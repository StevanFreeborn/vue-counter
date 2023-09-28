<script setup lang="ts">
import { ref } from 'vue';
const count = ref(0);
const increase = () => count.value++;
const decrease = () => count.value--;
</script>

<template>
  <main>
    <div>
      <h4>The current count is...</h4>
      <h1>{{ count }}</h1>
      <div class="button-container">
        <button @click="decrease">Decrement</button>
        <button @click="increase">Increment</button>
      </div>
    </div>
  </main>
</template>

<style scoped>
* {
  box-sizing: border-box;
}

html,
body {
  margin: 0;
  padding: 0;
  height: 100%;
}

main {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  background-color: aliceblue;
}

main > div {
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
