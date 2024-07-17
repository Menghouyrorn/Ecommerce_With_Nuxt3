<template>
  <div class="h-screen mt-2 flex flex-col gap-y-8">
    <h1 class="text-7xl text-center h-[10%]">FASHIONABLE COMFORT BLEND</h1>
    <div class="flex h-[90%]">
      <div class="w-[50%] h-full">
        <Card
          class="w-full h-full rounded-sm shadow-none border-none bg-transparent min-w-sm"
        >
          <CardContent class="h-full">
            <div class="flex h-full gap-y-4 flex-col">
              <img
                class="w-full h-[100%]"
                src="https://www.shutterstock.com/image-photo/beautiful-brunette-woman-natural-makeup-600nw-1781009285.jpg"
              />
              <div class="flex flex-col gap-y-3 p-0 w-full">
                <p>
                  Premium Photo | Fashion model and black woman in studio for
                  creative clothes and posing in power
                </p>
                <Button class="bg-[#8c614f] w-full">Shop Now</Button>
              </div>
            </div>
          </CardContent>
        </Card>
      </div>
      <div class="w-[50%] min-w-sm h-full">
        <img
          class="w-[100%] h-[96%]"
          src="https://img.freepik.com/free-photo/portrait-pretty-blonde-model-sitting-table-white-casual-warm-knitted-sweater-black-hat_273443-2244.jpg?size=626&ext=jpg&ga=GA1.1.1141335507.1719273600&semt=ais_user"
        />
      </div>
    </div>
  </div>
</template>

<script setup>
import { CardContent, Card } from "~/components/ui/card";
</script>

<style lang="scss" scoped>
</style>