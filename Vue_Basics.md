# Vue.js Example Component

This is a simple Vue 3 component written in the Composition API. It displays a counter with increment and reset buttons.

##  Component: `Counter.vue`

```vue
<template>
  <div class="counter">
    <h2>Count: {{ count }}</h2>
    <button @click="increment">Increment</button>
    <button @click="reset">Reset</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)

function increment() {
  count.value++
}

function reset() {
  count.value = 0
}
</script>

<style scoped>
.counter {
  text-align: center;
  padding: 1rem;
  border: 1px solid #ccc;
  border-radius: 8px;
}
button {
  margin: 0.5rem;
  padding: 0.5rem 1rem;
}
</style>
