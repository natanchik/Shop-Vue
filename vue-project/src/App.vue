<script lang="ts">
import { defineComponent } from 'vue'
import HeaderEl from './components/HeaderEl.vue'

export default defineComponent({
  name: 'App',
  components: {
    HeaderEl
  }
})
</script>

<template>
  <main class="w-4/5 h-full m-auto my-10 bg-white rounded-xl shadow-xl">
    <HeaderEl />
  </main>
</template>

<style scoped></style>
