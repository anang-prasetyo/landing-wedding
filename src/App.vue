<script setup>
import { RouterView } from 'vue-router'
import NavBar from './components/NavBar.vue';
</script>

<template>
  <header>
    <div class="wrapper">
      <nav-bar />
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
@media (min-width: 1024px) {

}
</style>
