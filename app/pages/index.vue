<template>
  <div>
    <section class="bg-linear-to-br from-blue-700 via-indigo-700 to-purple-700 text-white">
      <div class="max-w-6xl mx-auto px-6 py-24 text-center">
        <h2 class="text-4xl md:text-5xl font-extrabold">
          Student Information Website
        </h2>
        <p class="mt-4 text-lg text-blue-100 max-w-2xl mx-auto">
          A simple website built with reusable Vue components and props.
        </p>
        <div class="mt-8 flex flex-wrap justify-center gap-4">
          <AppButton label="View Students" color="white" to="/students" />
          <AppButton label="Learn More" color="green" to="#about" />
        </div>
      </div>
    </section>

    <section id="about" class="max-w-6xl mx-auto px-6 py-16">
      <h3 class="text-3xl font-bold text-center mb-10">What this project shows</h3>
      <div class="grid gap-6 md:grid-cols-3">
        <InfoCard icon="🧩" title="Reusable Components"
                  description="Header, footer and cards are written once and used on every page." />
        <InfoCard icon="📦" title="Props"
                  description="Data like name and course is passed into components using props." />
        <InfoCard icon="🎨" title="Customizable Buttons"
                  description="The same button changes its label, color and link through props." />
      </div>
    </section>
  </div>
</template>