<template>
  <div class="xl:w-1/4 md:w-1/2 p-4">
        <div class="bg-gray-100 p-6 rounded-lg">
          <img class="h-64 rounded w-full object-cover object-center mb-6" :src="getPictureUrl(book.image.url)" alt="content">
          <h3 class="tracking-widest text-blue-900 text-xs font-medium title-font">{{book.authors[0].name}}</h3>
          <h2 class="text-lg text-gray-900 font-medium title-font mb-4">{{book.name}}</h2>
          <div class="flex">
            <img src="star-full.svg" alt="">
            <img src="star-full.svg" alt="">
            <img src="star-full.svg" alt="">
            <img src="star-full.svg" alt="">
            <img src="star-empty.svg" alt="">
          </div>
        </div>
      </div>
</template>

<script>
export default {
    props: [
      'book'
    ],
    methods: {
      getPictureUrl(relativeUrl) {
        return `${process.env.MY_HEROKU_URL || "http://localhost:1337"}${relativeUrl}`;
      }
    }
}
</script>

<style>

</style>