---
layout: default
title: "QA × IA – Alberto Barragán"
---
<section class="max-w-6xl mx-auto px-4 py-24 flex flex-col lg:flex-row items-center gap-10">
  <div class="flex-1">
    <h1 class="text-4xl sm:text-5xl font-extrabold mb-6 leading-tight">Calidad de Software &amp; <span class="text-sky-600">Inteligencia Artificial</span></h1>
    <p class="text-lg mb-8">Destripando QA, automatización E2E y modelos IA con ejemplos del mundo real. Cada semana, un nuevo artículo directamente desde mi laboratorio.</p>
    <a href="/blog/" class="inline-block bg-sky-600 text-white px-6 py-3 rounded-xl shadow hover:bg-sky-700 transition">Ir al Blog</a>
  </div>
  <div class="flex-1">
    <img src="/assets/images/logo.png" alt="Ilustración QA & IA" class="w-full">
  </div>
</section>

<section class="bg-neutral-100 dark:bg-neutral-800 py-16">
  <div class="max-w-6xl mx-auto px-4">
    <h2 class="text-3xl font-bold mb-8">Últimos artículos</h2>
    <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
      {% for post in site.posts limit:6 %}
      <a href="{{ post.url | relative_url }}" class="block bg-white dark:bg-neutral-900/80 rounded-2xl shadow p-6 hover:-translate-y-1 transition">
        <h3 class="text-xl font-bold mb-2">{{ post.title }}</h3>
        <p class="text-sm text-neutral-500 mb-4">{{ post.date | date: "%d %b %Y" }}</p>
        <p class="line-clamp-3 text-neutral-700 dark:text-neutral-300">{{ post.excerpt | strip_html | truncate: 120 }}</p>
      </a>
      {% endfor %}
    </div>
  </div>
</section>

---