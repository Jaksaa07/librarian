<template>
  <div>
      <div class="container px-4 mx-auto my-8 text-blue-900">
        <div class="grid grid-cols-1 mt-5 mx-7">
          <label class="uppercase md:text-sm text-xs text-gray-500 text-light font-semibold">Search</label>
          <input class="py-2 px-3 rounded-lg border-2 border-gray-500 mt-1 focus:outline-none focus:ring-2 focus:ring-blue-900 focus:border-transparent" type="text" placeholder="Search" />
        </div>
        <div class="grid grid-cols-1 mt-5 mx-7">
            <label class="uppercase md:text-sm text-xs text-gray-500 text-light font-semibold">Selection</label>
            <select class="py-2 px-3 rounded-lg border-2 border-gray-500 mt-1 focus:outline-none focus:ring-2 focus:ring-blue-900 focus:border-transparent">
              <option>Fiction</option>
              <option>Nonfiction</option>
            </select>
        </div>
      </div>
      <BookList />
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>