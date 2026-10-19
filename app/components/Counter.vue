<template>
  <div class="not-prose my-6 rounded-lg border border-gray-200 bg-white p-4 shadow-sm">
    <h3 class="mb-3 text-lg font-semibold">
      Counter: {{ count }}
    </h3>
    <div class="flex gap-2">
      <button
        class="rounded-md bg-emerald-600 px-4 py-2 text-sm font-medium text-white hover:bg-emerald-700 active:bg-emerald-800"
        @click="increment"
      >
        Increment
      </button>
      <button
        class="rounded-md bg-gray-200 px-4 py-2 text-sm font-medium text-gray-800 hover:bg-gray-300 active:bg-gray-400"
        @click="decrement"
      >
        Decrement
      </button>
    </div>
  </div>
</template>

<script setup lang="ts">
const count = ref(0)

const increment = () => {
  count.value++
}

const decrement = () => {
  count.value--
}
</script>
