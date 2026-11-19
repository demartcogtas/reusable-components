<script setup>
const props = defineProps({
  name: { type: String, required: true },
  course: { type: String, required: true },
  year: { type: String, default: '1st Year' },
  email: { type: String, default: 'N/A' }
})

const initials = computed(() =>
  props.name.split(' ').map(w => w[0]).slice(0, 2).join('').toUpperCase()
)
</script>

<template>
  <div class="bg-white rounded-2xl shadow-md border border-slate-100 overflow-hidden
              hover:shadow-xl hover:-translate-y-1 transition">
    <div class="h-20 bg-lineart-to-r from-blue-600 to-indigo-600"></div>
    <div class="px-6 pb-6">
      <div class="-mt-10 w-20 h-20 rounded-full bg-blue-100 border-4 border-white shadow
            flex items-center justify-center text-2xl font-bold text-blue-700">
        {{ initials }}
      </div>
      <h3 class="mt-3 text-xl font-bold text-slate-800">{{ name }}</h3>
      <p class="text-slate-600">{{ course }}</p>
      <span class="inline-block mt-2 text-xs font-semibold bg-blue-100 text-blue-700 px-3 py-1 rounded-full">
        {{ year }}
      </span>
      <p class="mt-3 text-sm text-slate-500">✉️ {{ email }}</p>
    </div>
  </div>
</template>