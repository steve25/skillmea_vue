<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import TheNavigation from './components/TheNavigation.vue'
</script>

<template>
  <header>
    <TheNavigation></TheNavigation>
  </header>

  <main class="content">
    <RouterView />
  </main>

</template>

<style src="@/assets/scss/main.scss"></style>
