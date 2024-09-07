<script setup>
import TaskList from "../components/TaskList.vue";
import { ref } from "vue";
const tasks = ref([
  { id: 1, title: "gym", completed: true },
  { id: 2, title: "study", completed: false },
  { id: 3, title: "sleep", completed: false },
  { id: 4, title: "laundry", completed: true },
  { id: 5, title: "cafee", completed: false },
  { id: 6, title: "class", completed: false },
]);

function deleteItem(taskId) {
  tasks.value = tasks.value.filter((task) => task.id !== taskId);
  console.log(tasks.value);
}
</script>

<template>
  <TaskList :tasks="tasks" @deleteItem="deleteItem($event)" />
</template>
