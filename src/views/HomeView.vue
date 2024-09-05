<script setup>
import TaskList from "../components/TaskList.vue";
import { ref } from "vue";
const tasks = ref([
  { id: 1, title: "gym", complited: true },
  { id: 2, title: "study", complited: false },
]);
</script>

<template>
  <TaskList :tasks="tasks" />
</template>
