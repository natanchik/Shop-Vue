<template>
  <div class="fixed top-0 left-0 w-full h-full z-10 bg-slate-400">
    <div class="fixed top-0 right-0 z-20 p-7 bg-white w-full sm:w-96 h-full">
      <h2 class="font-bold text-2xl mb-4">Cart</h2>
      <div
        class="flex flex-wrap justify-between gap-4 w-full h-2/3 max-[655px]:justify-center overflow-y-scroll"
      >
        <CartItem
          :image="card.id"
          :text="card.title"
          :price="card.price"
          v-for="card in SNEAKERS"
          :key="card.id"
        />
      </div>
      <div class="flex flex-col gap-5 p-7 justify-between items-stretch h-20 text-base">
        <span class="flex justify-between">
          <p>Total Price:</p>
          <span class="flex-1 border-b border-dashed" />
          <p>1250</p>
        </span>
        <span class="flex justify-between">
          <p>Tax 5%:</p>
          <span class="flex-1 border-b border-dashed" />
          <p>50</p>
        </span>
        <button
          class="border w-full h-14 p-4 rounded-[18px] bg-lime-400 text-white font-semibold hover:bg-lime-500 transition"
        >
          Place an order
        </button>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import CartItem from './CartItem.vue'
import SNEAKERS from '../sneakers'
</script>
