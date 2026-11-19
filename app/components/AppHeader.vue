<template>
  <header class="sticky top-0 z-10 bg-slate-900/95 backdrop-blur text-white shadow-lg">
    <nav class="max-w-6xl mx-auto flex items-center justify-between px-6 py-4">
      <NuxtLink to="/" class="flex items-center gap-2 text-xl font-extrabold">
        <span class="bg-blue-500 rounded-lg px-2 py-1">🎓</span>
        Student<span class="text-blue-400">Info</span>
      </NuxtLink>
      <div class="flex gap-2">
        <NuxtLink to="/" exact-active-class="bg-blue-600"
                  class="px-4 py-2 rounded-lg hover:bg-slate-700 transition">Home</NuxtLink>
        <NuxtLink to="/students" exact-active-class="bg-blue-600"
                  class="px-4 py-2 rounded-lg hover:bg-slate-700 transition">Students</NuxtLink>
      </div>
    </nav>
  </header>
</template>