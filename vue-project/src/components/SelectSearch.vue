<template>
  <div class="flex flex-wrap gap-4 justify-end">
    <select
      class="w-[210px] border rounded-xl px-3 py-2 focus:border-slate-400 focus:shadow-sm outline-none"
    >
      <option>Name</option>
      <option>Price (cheap)</option>
      <option>Price (expensive)</option>
    </select>
    <span class="relative">
      <img :src="'./search.svg'" alt="Search" class="absolute top-[13px] left-2 h-4 w-4" />
      <input
        class="border w-[210px] rounded-xl pr-3 py-2 pl-8 focus:border-slate-400 focus:shadow-sm outline-none"
        placeholder="Search..."
      />
    </span>
  </div>
</template>
