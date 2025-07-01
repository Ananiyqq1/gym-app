<script setup>
import Layout from './components/layouts/Layout.vue';
import Dashboard from './components/pages/Dashboard.vue';
import Welcome from './components/pages/Welcome.vue'
import Workout from './components/pages/Workout.vue';

const selectedDisplay = 3;
</script>

<template>

<Layout>
  <!-- P1 -->
  <Welcome v-if="selectedDisplay === 1" />
  <!-- P2 -->
  <Dashboard v-if="selectedDisplay === 2" />
  <!-- P3 -->
  <Workout v-if="selectedDisplay === 3" />

</Layout>

</template>

<style scoped>

</style>