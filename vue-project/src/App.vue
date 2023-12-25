<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <main class="w-4/5 h-full m-auto my-10 bg-white rounded-xl shadow-xl">
    <h1>Vue Title</h1>
    <HelloWorld title="Title" :price="5">
      <h1>Added title</h1>
    </HelloWorld>
  </main>
</template>

<style scoped></style>
