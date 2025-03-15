<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div class="min-h-screen bg-gray-100 dark:bg-gray-900">
    <header class="bg-white dark:bg-gray-800 shadow-lg">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-6">
        <div class="flex items-center justify-between">
          <div class="flex items-center space-x-4">
            <a href="https://vite.dev" target="_blank" class="hover:opacity-80 transition-opacity">
              <img src="/vite.svg" class="h-12 w-12" alt="Vite logo" />
            </a>
            <a href="https://vuejs.org/" target="_blank" class="hover:opacity-80 transition-opacity">
              <img src="./assets/vue.svg" class="h-12 w-12" alt="Vue logo" />
            </a>
          </div>
          <h1 class="text-2xl font-bold text-gray-900 dark:text-white">
            Habit Tracker
          </h1>
        </div>
      </div>
    </header>

    <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8">
      <HelloWorld msg="Vite + Vue" />
    </main>
  </div>
</template>

<style scoped>
.logo {
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
