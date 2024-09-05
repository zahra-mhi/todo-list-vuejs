<script setup>
const props = defineProps({
  task: Object,
});
</script>
<template>
  <div class="bg-light mb-3 ps-2 py-1 border rounded">
    <div class="form-check">
      <input class="form-check-input" type="checkbox"  checked />
      <label class="form-check-label"> {{ task.title }} </label>
    </div>
  </div>
</template>