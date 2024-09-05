<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <nav class="navbar navbar-expand navbar-light bg-light mb-4">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">ToDo</a>
        <div class="navbar-nav">
          <RouterLink class="nav-link" to="/">Home</RouterLink>
          <a class="nav-link" href="#">About</a>
        </div>
      </div>
    </nav>
  </header>

  <RouterView />
</template>

<style scoped>
</style>
