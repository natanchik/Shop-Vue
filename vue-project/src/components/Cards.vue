<template>
  <div class="flex flex-wrap justify-between gap-4 w-full max-[655px]:justify-center">
    <Card
      :image="card.id"
      :text="card.title"
      :price="card.price"
      v-for="card in SNEAKERS"
      :key="card.id"
    />
  </div>
</template>

<script setup lang="ts">
import Card from './Card.vue'
// import { type SneakerType } from '../sneakers'
// import { type PropType } from 'vue'
import SNEAKERS from '../sneakers'

// defineProps({
//   cards: Array as PropType<SneakerType[]>
// })
</script>
