<template>
  <div
    class="rounded-2xl p-5"
    :class="highlight ? 'bg-lime-200' : 'bg-white'"
  >
    <p class="text-sm text-gray-500 mb-2">{{ title }}</p>
    <h2 class="text-4xl font-bold">{{ value }}</h2>
    <p class="text-xs text-gray-500 mt-1">{{ subtitle }}</p>

    <div class="flex gap-1 mt-4">
      <div
        v-for="i in 10"
        :key="i"
        class="w-4 h-6 rounded"
        :class="i <= bars ? 'bg-black' : 'bg-black/10'"
      ></div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  value: String,
  subtitle: String,
  bars: Number,
  highlight: Boolean
})
</script>
