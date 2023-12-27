<template>
  <div
    class="relative border w-[210px] h-[260px] rounded-[40px] p-7 flex flex-col gap-4 justify-center transition hover:drop-shadow-xl"
  >
    <img
      :src="favor ? './like-2.svg' : './like-1.svg'"
      @click="addFavor"
      alt="Favorites"
      class="absolute top-7 left-7 w-8 h-8 border"
    />
    <img :src="url" alt="Sneacker" class="w-[133px] h-[112px]" />
    <p class="text-sm">{{ text }}</p>
    <span class="text-slate-400 flex justify-between items-start">
      <span class="flex flex-col">
        <p>PRICE:</p>
        <p class="font-bold text-slate-950">{{ price }} coins</p>
      </span>
      <img
        :src="choice ? '/checked.svg' : '/plus.svg'"
        alt="Plus"
        class="border h-8 w-8 rounded shadow-md"
        @click="choose"
      />
    </span>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const props = defineProps({
  image: Number,
  text: String,
  price: Number
})

const url = './sneakers/sneakers-' + props.image + '.jpg'
let choice = ref(false)
let favor = ref(false)

function addFavor() {
  favor.value = !favor.value
}

function choose() {
  choice.value = !choice.value
}
</script>
