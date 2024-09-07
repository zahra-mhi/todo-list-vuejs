<script setup>
const props = defineProps({
  task: Object,
});
</script>

<template>
  <div class="bg-light mb-3 ps-2 py-1 border rounded">
    <div class="form-check" :class="{ completed: task.completed }">
      <input
        class="form-check-input"
        :class="{ completed: task.completed }"
        type="checkbox"
        :checked="task.completed"
        @change="task.completed = !task.completed"
      />
      <label class="form-check-label" :class="{ completed: task.completed }">
        {{ task.title }}
      </label>
    </div>
  </div>
</template>

<style scoped>
.completed {
  text-decoration: line-through;
  opacity: 0.6;
}
</style>