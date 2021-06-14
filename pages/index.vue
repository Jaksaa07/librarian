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
export default {
  data() {
    return {
      books: []
    }
  },
  async fetch() {
    this.books = await fetch(`${process.env.MY_HEROKU_URL || "http://localhost:1337"}/books`).then(res =>
      res.json()
    )
  },
};
</script>

