<script setup>
import { ref, reactive } from 'vue'
const location = reactive({
  name: 'Dhaka',
  weather: 'Sunny',
})

function changeLocation(newLocation) {
  location.name = newLocation
}
</script>

<template>
  <section class="container mx-auto flex items-center flex-col">
    <h1 class="text-center text-2xl py-10">Events & Reactivity in Vue.js</h1>
    <div class="container mx-auto flex space-x-5 justify-center m-5">
      <button
        class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
        @click="changeLocation('Dhaka')"
      >
        Dhaka
      </button>
      <button
        class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
        @click="changeLocation('Rajshahi')"
      >
        Rajshahi
      </button>
      <button
        class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
        @click="changeLocation('Khulna')"
      >
        Khulna
      </button>
      <button
        class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded"
        @click="changeLocation('Chattagram')"
      >
        Chattagram
      </button>
    </div>
    <h1 class="text-2xl m-10">Current Location is {{ location.name }}</h1>
  </section>
</template>

<style scoped></style>
