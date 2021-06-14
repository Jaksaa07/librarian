<template>
  <div class="bg-blue-900 text-white shadow-lg">
    <div class="container mx-auto px-2 flex-col">
      <div class="flex justify-between">
        <img src="../static/logo.svg" alt="">
        <img @click="navMenu = !navMenu" class="mr-2" src="../static/menu.svg" alt="">
      </div>
      <nav>
        <ul v-if="navMenu" class="flex flex-col p-2 gap-4">
          <!-- <input class="p-2 ml-4 rounded-lg" type="text" placeholder="Search by author or title" /> -->
          <li @click="navMenu = false" class="text-lg"><NuxtLink to="/">Home</NuxtLink></li>
          <li @click="navMenu = false" class="text-lg"><NuxtLink to="/books">Categories</NuxtLink></li>
          <li @click="navMenu = false" class="text-lg"><NuxtLink to="/blog">Blog</NuxtLink></li>
          <li @click="navMenu = false" class="text-lg"><NuxtLink to="/contact">Contact</NuxtLink></li>
          <li @click="navMenu = false" class="text-lg"><NuxtLink to="/login">Sign In</NuxtLink></li>
          <li @click="navMenu = false" class="text-lg mb-2"><NuxtLink to="/register">Sign Up</NuxtLink></li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      navMenu: false,
    }
  }
};
</script>

<style lang="scss" scoped>
</style>