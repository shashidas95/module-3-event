<script setup>
const items = [
  {
    id: 1,

    title: 'Item 1',

    description: 'Description for Item 1',
  },

  {
    id: 2,

    title: 'Item 2',

    description: 'Description for Item 2',
  },

  {
    id: 3,

    title: 'Item 3',

    description: 'Description for Item 3',
  },

  {
    id: 4,

    title: 'Item 4',

    description: 'Description for Item 4',
  },

  {
    id: 5,

    title: 'Item 5',

    description: 'Description for Item 5',
  },

  {
    id: 6,

    title: 'Item 6',

    description: 'Description for Item 6',
  },
]
</script>

<template>
  <section
    class="mx-auto container flex items-center text-center flex-col space-y-2"
  >
    <ul class="list-disc p-5 w-100" v-for="item in items" :key="items.id">
      <li class="text-start w-full">{{ item.id }} .{{ item.title }}</li>
      <p>{{ item.description }}</p>
    </ul>
  </section>
</template>

<style scoped></style>
