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
  <div v-for="todo in todos" data-test="todo">{{ todo.text }}</div>
</template>
