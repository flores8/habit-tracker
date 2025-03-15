<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <div class="bg-white dark:bg-gray-800 rounded-lg shadow-md p-6">
    <h1 class="text-3xl font-bold text-gray-900 dark:text-white mb-6">{{ msg }}</h1>

    <div class="space-y-6">
      <div class="bg-gray-50 dark:bg-gray-700 rounded-lg p-4">
        <button 
          type="button" 
          @click="count++"
          class="px-4 py-2 bg-blue-500 hover:bg-blue-600 text-white rounded-md transition-colors duration-200"
        >
          Count is {{ count }}
        </button>
        <p class="mt-4 text-gray-600 dark:text-gray-300">
          Edit
          <code class="bg-gray-200 dark:bg-gray-600 px-2 py-1 rounded text-sm">components/HelloWorld.vue</code>
          to test HMR
        </p>
      </div>

      <div class="space-y-4">
        <p class="text-gray-600 dark:text-gray-300">
          Check out
          <a 
            href="https://vuejs.org/guide/quick-start.html#local" 
            target="_blank"
            class="text-blue-500 hover:text-blue-600 underline"
          >
            create-vue
          </a>
          , the official Vue + Vite starter
        </p>
        <p class="text-gray-600 dark:text-gray-300">
          Learn more about IDE Support for Vue in the
          <a
            href="https://vuejs.org/guide/scaling-up/tooling.html#ide-support"
            target="_blank"
            class="text-blue-500 hover:text-blue-600 underline"
          >
            Vue Docs Scaling up Guide
          </a>
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
