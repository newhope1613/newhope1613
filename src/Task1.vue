<script setup>
import { ref } from 'vue';

const inputTask = ref('');
const items = ref([]);

const addTask = () => {
  items.value.push(inputTask.value);
  inputTask.value = '';
};

const addTaskWithText = (text) => {
  items.value.push(text);
  inputTask.value = '';
};
</script>

<template>
  Список задач:
  <input type="text" v-model="inputTask" />
  <button type="button" @click="addTask">Добавить</button>
  <br />
  Hello
  <ul>
    <li v-for="item in items">{{ item }}</li>
  </ul>
</template>
