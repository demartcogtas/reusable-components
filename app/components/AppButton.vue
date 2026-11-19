<script setup>
const props = defineProps({
  label: { type: String, default: 'Click Me' },
  color: { type: String, default: 'blue' },
  to: { type: String, default: '' }
})

const colors = {
  blue: 'bg-blue-600 hover:bg-blue-700 shadow-blue-600/30',
  green: 'bg-emerald-600 hover:bg-emerald-700 shadow-emerald-600/30',
  red: 'bg-rose-600 hover:bg-rose-700 shadow-rose-600/30',
  white: 'bg-white text-blue-700 hover:bg-blue-50 shadow-black/10'
}

const classes = computed(() => [
  colors[props.color] || colors.blue,
  props.color === 'white' ? '' : 'text-white',
  'inline-block px-6 py-3 rounded-xl font-semibold shadow-lg',
  'transition hover:-translate-y-0.5 active:translate-y-0'
])
</script>

<template>
  <NuxtLink v-if="to" :to="to" :class="classes">{{ label }}</NuxtLink>
  <button v-else :class="classes">{{ label }}</button>
</template>