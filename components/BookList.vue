<template>
  <div class="text-blue-900 container my-4 px-2 mx-auto">
    <div class="flex flex-wrap -m-4 px-8">
      <Card v-for="book in books" :key="book.id" :book="book"/>
    </div>
  </div>
</template>

<script>
export default {
  props: [
    'books'
  ],
}
</script>

<style>

</style>