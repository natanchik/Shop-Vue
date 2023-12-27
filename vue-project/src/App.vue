<script lang="ts">
import { defineComponent } from 'vue'
import HeaderComp from './components/HeaderComp.vue'
import Cards from './components/Cards.vue'
import Drawer from './components/Drawer.vue'

export default defineComponent({
  name: 'App',
  components: {
    HeaderComp,
    Cards,
    Drawer
  }
})
</script>

<template>
  <main class="flex flex-col gap-10 w-4/5 h-full m-auto p-11 my-10 bg-white rounded-xl shadow-xl">
    <HeaderComp />
    <h1 class="font-bold text-3xl">All sneakers</h1>
    <Cards />
    <Drawer />
  </main>
</template>

<style scoped></style>
