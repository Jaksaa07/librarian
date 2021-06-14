<template>
  <div class="bg-white shadow rounded-lg p-6">
    <div class="mb-8 flex justify-between">
      <h1 class="font-bold text-blue-900 text-2xl">Welcome to Librarian!</h1>
      <NuxtLink to='/' class="mt-2 text-gray-600 text-sm underline">Back to home</NuxtLink>
    </div>
    <div class="grid lg:grid-cols-2 gap-6">
      <div class="border focus-within:border-blue-500 focus-within:text-blue-500 transition-all duration-500 relative rounded p-1">
        <div class="-mt-4 absolute tracking-wider px-1 uppercase text-xs">
          <p>
            <label for="email" class="bg-white text-gray-600 px-1">Email *</label>
          </p>
        </div>
        <p>
          <input id="email" autocomplete="false" tabindex="0" type="text" class="py-1 px-1 outline-none block h-full w-full">
        </p>
      </div>
      <div class="border focus-within:border-blue-500 focus-within:text-blue-500 transition-all duration-500 relative rounded p-1">
        <div class="-mt-4 absolute tracking-wider px-1 uppercase text-xs">
          <p>
            <label for="password" class="bg-white text-gray-600 px-1">Password *</label>
          </p>
        </div>
        <p>
          <input id="password" autocomplete="false" tabindex="0" type="password" class="py-1 px-1 outline-none block h-full w-full">
        </p>
      </div>
    </div>
    <div class="border-t mt-6 pt-3 flex justify-between">
      <button class="rounded-lg text-gray-100 px-3 py-1 bg-blue-400 focus:outline-none hover:shadow-inner hover:bg-blue-700 transition-all duration-300">
        Sign in
      </button>
      <NuxtLink class="text-gray-600 mt-2 focus:underline" to="/register">Don't have an account?</NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
    layout: 'auth'
}
</script>

<style>

</style>