<template>
  <div
    class="not-prose my-6 flex items-center rounded-lg border-2 bg-white p-4 shadow-md transition duration-200 hover:-translate-y-0.5 hover:shadow-lg"
    :style="{ 'border-color': color }"
  >
    <slot></slot>
  </div>
</template>

<script setup lang="ts">
const { color } = defineProps({
  color: {
    type: String,
    default: 'orange'
  }
})
</script>
