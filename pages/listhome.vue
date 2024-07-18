<template>
  <div class="w-full h-screen mt-40">
    <h1 class="uppercase text-4xl text-center m-auto w-[30%]">
      find exactly what you need
    </h1>

    <div class="flex flex-col gap-y-24 w-[82%] m-auto">
      <div class="flex gap-4 justify-center mt-16">
        <div v-for="data1 in data" :key="data1">
          <Card
            class="w-[290px] h-[330px] border-none bg-transparent shadow-none"
          >
            <CardContent
              class="bg-white shadow rounded-md w-full h-full flex items-center justify-center pt-6"
            >
              <img class="w-[90%] h-[90%]" :src="`${data1.image}`" alt="" />
            </CardContent>
            <CardFooter class="flex justify-end mt-2">
              <div class="text-end font-bold">
                <p>Hat</p>
                <p>$ 23.00</p>
              </div>
            </CardFooter>
          </Card>
        </div>
      </div>
      <div class="flex justify-end">
        <NuxtLink to="#" class="text-xl hover:underline">Load More </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script setup>
import { Get } from "~/services";

let data = [];
data = await Get({
  url: "https://fakestoreapi.com/products?sort=desc&limit=4",
})
  .then((data) => {
    return data;
  })
  .catch((err) => console.log(err));
</script>

<style lang="scss" scoped>
</style>