<template>
  <div>
    <Hero />
    <div class="flex justify-between px-4 text-blue-900 container my-4 mx-auto">
      <p class="font-medium text-xl">List</p>
      <NuxtLink to='/books'>View All</NuxtLink>
    </div>
    <BookList :books="books" />
  </div>
</template>

<script>
import booksQuery from '../apollo/queries/books'
export default {
  data() {
    return {
      books: []
    }
  },
  apollo: {
    books: {
      prefetch: true,
      query: booksQuery
    }
  }
};
</script>

