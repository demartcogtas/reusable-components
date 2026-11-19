<template>
  <div class="max-w-6xl mx-auto px-6 py-12">
    <div class="text-center mb-10">
      <h2 class="text-3xl md:text-4xl font-extrabold">Our Students</h2>
      <p class="text-slate-600 mt-2">Each card is the same component with different props.</p>
    </div>

    <div class="grid gap-6 md:grid-cols-3">
      <StudentCard name="Eleanore Barata" course="BS Information Technology"
                   year="3rd Year" email="eleanore@example.com" />
      <StudentCard name="Maria Santos" course="BS Computer Science"
                   year="3rd Year" email="maria@example.com" />
      <StudentCard name="Pedro Reyes" course="BS Information Systems"
                   year="1st Year" email="pedro@example.com" />
    </div>

    <div class="mt-12 text-center">
      <AppButton label="Back to Home" color="blue" to="/" />
    </div>
  </div>
</template>