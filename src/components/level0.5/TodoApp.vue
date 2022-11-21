<script setup>
import { ref } from 'vue';

const todos = ref([
  {
    id: 1,
    text: 'Learn Vue.js 3',
    completed: false,
  },
]);
</script>
<template>
  <div data-test="todo">
    <div v-for="todo in todos" :key="todo.id">{{ todo.text }}</div>
  </div>
</template>
