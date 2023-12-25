<!-- <script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    title: String,
    price: Number
  },
  data() {
    return {
      count: 0
    }
  },
  methods: {
    increment() {
      this.count++
    }
  }
})
</script> -->

<script setup lang="ts">
import { ref } from 'vue'

defineProps({
  title: String,
  price: Number
})

let count = ref(0)

function increment() {
  count.value++
}
</script>

<template>
  <div>
    <h1>{{ count }}</h1>
    <p>{{ title }}</p>
    <p>{{ price }}</p>
    <button class="border" @click="increment">Add</button>
    <input @keyup.ctrl.enter="increment" />
    <slot></slot>
  </div>
</template>
