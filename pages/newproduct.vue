<template>
  <div class="h-screen w-full p-4">
    <div>
      <h1 class="text-6xl uppercase p-4">What new in store?</h1>
    </div>
    <div class="flex items-center justify-center gap-6" >
      <div v-for="data1 in data" :key="`${data1.id}`">
        <div class="border rounded border-black">
          <img
            :src="`${data1.image}`"
            class="w-[450px] rounded h-[470px]"
            alt=""
          />
        </div>
      </div>
    </div>

    <div
      class="flex justify-end items-center pt-10 pb-10 pr-7 underline text-2xl"
    >
      <NuxtLink to="#">Watch more !</NuxtLink>
    </div>
  </div>
</template>

<script setup>
import { Get } from "../services";
let data = [];
data = await Get({
  url: "https://fakestoreapi.com/products?sort=desc&limit=3",
})
  .then((data) => {
    return data;
  })
  .catch((error) => {
    console.log(error);
  });
console.log(data);
</script>

<style lang="scss" scoped>
</style>