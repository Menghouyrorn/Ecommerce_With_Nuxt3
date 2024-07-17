<template>
  <div class="bg-[#fffae7]">
    <div
      class="w-full p-2 h-[8vh] border-b-[3px] border-[#e6e6e6] flex items-center justify-between"
    >
      <div class="flex gap-6 pl-6">
        <NuxtLink class="hover:underline transition-all cursor-pointer"
          >BRANDS</NuxtLink
        >
        <NuxtLink class="hover:underline transition-all cursor-pointer"
          >MAN'S</NuxtLink
        >
        <NuxtLink class="hover:underline transition-all cursor-pointer"
          >WOMAN'S</NuxtLink
        >
      </div>
      <div class="text-2xl">BTee<span class="text-[#52392f]">Co</span></div>
      <div class="flex items-center gap-4 pr-6">
        <NuxtLink to="#"
          ><Icon name="ic:baseline-search" class="text-xl"
        /></NuxtLink>
        <NuxtLink to="#"
          ><Icon name="material-symbols:add-shopping-cart" class="text-xl"
        /></NuxtLink>
        <NuxtLink to="#"
          ><Icon name="material-symbols:account-circle" class="text-xl"
        /></NuxtLink>
      </div>
    </div>
    <slot />
  </div>
</template>

<script setup>
</script>

<style lang="scss" scoped>
</style>