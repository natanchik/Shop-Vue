<template>
  <div class="flex justify-between p-11">
    <div class="flex gap-4 items-center">
      <img :src="'./logo.png'" alt="Logo" class="w-10 h-10" />
      <div>
        <h2 class="text-xl font-bold">REACT SNEAKERS</h2>
        <p class="text-[#9D9D9D]">Best sneackers shop</p>
      </div>
    </div>

    <ul class="flex gap-8 items-center">
      <li
        class="flex flex-nowrap gap-2 cursor-pointer text-[#5C5C5C] font-semibold hover:text-slate-800"
      >
        <img :src="'./cart.svg'" alt="Total price" />
        <p>1205 coins</p>
      </li>
      <li class="flex flex-nowrap gap-2 cursor-pointer text-[#5C5C5C] hover:text-slate-800">
        <img :src="'./heart.svg'" alt="Favorites" />
        <p>Favorites</p>
      </li>
      <li class="flex flex-nowrap gap-2 cursor-pointer text-[#5C5C5C] hover:text-slate-800">
        <img :src="'./profile.svg'" alt="Profile" />
        <p>Profile</p>
      </li>
    </ul>
  </div>
</template>

<script setup lang="ts"></script>
