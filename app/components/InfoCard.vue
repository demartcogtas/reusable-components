<script setup>
defineProps({
  title: String,
  description: String,
  icon: { type: String, default: '📘' }
})
</script>

<template>
  <div class="bg-white rounded-2xl p-6 shadow-md border border-slate-100
              hover:shadow-xl hover:-translate-y-1 transition">
    <div class="text-3xl mb-3">{{ icon }}</div>
    <h3 class="font-bold text-lg text-slate-800">{{ title }}</h3>
    <p class="text-slate-600 mt-1">{{ description }}</p>
  </div>
</template>