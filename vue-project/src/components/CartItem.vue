<template>
  <div
    class="relative border w-[325px] h-[119px] rounded-[20px] p-7 flex gap-4 justify-between items-center transition hover:drop-shadow-xl"
  >
    <div class="flex items-end justify-start gap-5">
      <img :src="url" alt="Sneacker" class="w-[70px] h-[70px]" />
      <span class="text-slate-400 flex flex-col gap-2 justify-center items-start w-[160px] text-sm">
        <p class="text-sm">{{ text }}</p>
        <p class="font-bold text-slate-950">{{ price }} coins</p>
      </span>
    </div>
    <img relative top-50 :src="'/close.svg'" alt="Close" class="border h-8 w-8 rounded shadow-md" />
  </div>
</template>

<script setup lang="ts">
const props = defineProps({
  image: Number,
  text: String,
  price: Number
})

const url = './sneakers/sneakers-' + props.image + '.jpg'
</script>
