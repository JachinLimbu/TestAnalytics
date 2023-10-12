<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <div class="container">
    <h3>This is a test website</h3>
    {{ count }}
    <div class="actions-container">
      <button @click="count++">+</button>
      <button @click="count--">-</button>
    </div>
  </div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.actions-container{
  display: flex;
}

button {
  background-color: rgb(165, 165, 165);
  color: rgb(235, 235, 235);
  margin: 2px 5px;
}
</style>
