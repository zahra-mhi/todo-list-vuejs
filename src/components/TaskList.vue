<script setup>
import Task from "../components/Task.vue";
const props = defineProps({
  tasks: Object,
});
</script>

<template>
  <div class="container bg-secondary p-4 rounded border">
    <h1 class="text-center mb-4">Task List</h1>
    <ul class="px-2">
      <div v-for="task in tasks" :key="task.id">
        <task :task="task" />
      </div>
    </ul>
  </div>
</template>