<script setup>
const features = [
  'Vue + Vite',
  'Tailwind CSS',
  'Nginx di STB',
  'Cloudflare Tunnel',
  'Siap CI/CD GitHub Actions'
]
</script>

<template>
  <main class="min-h-screen bg-slate-950 text-white">
    <section class="mx-auto flex min-h-screen max-w-5xl flex-col items-center justify-center px-6 text-center">
      <div class="mb-6 rounded-full border border-sky-400/30 bg-sky-400/10 px-4 py-2 text-sm text-sky-300">
        STB HG680P Mini Hosting
      </div>

      <h1 class="max-w-3xl text-4xl font-bold tracking-tight text-white md:text-6xl">
        Website Vue sederhana
        <span class="text-sky-400">online dari STB</span>
      </h1>

      <p class="mt-6 max-w-2xl text-base leading-8 text-slate-300 md:text-lg">
        Project ini dibuat dengan Vue, Vite, dan Tailwind CSS.
        Nanti setiap push ke GitHub branch main, website akan otomatis deploy ke STB.
      </p>

      <div class="mt-10 grid w-full gap-4 sm:grid-cols-2 lg:grid-cols-5">
        <div
          v-for="feature in features"
          :key="feature"
          class="rounded-2xl border border-slate-700 bg-slate-900/80 p-4 shadow-lg shadow-black/20"
        >
          <p class="text-sm font-semibold text-sky-300">
            {{ feature }}
          </p>
        </div>
      </div>

      <div class="mt-10 rounded-2xl border border-slate-700 bg-slate-900 p-6 text-left">
        <p class="text-sm text-slate-400">Status</p>
        <p class="mt-2 text-xl font-bold text-emerald-400">
          Deploy manual pertama siap dites 🚀
        </p>
      </div>
    </section>
  </main>
</template>