---
layout: default
title: "Blog"
---
<section class="max-w-6xl mx-auto px-4 py-12">
  <h1 class="text-3xl font-bold mb-8">Todas las entradas</h1>
  <div class="space-y-8">
    {% for post in site.posts %}
    <article class="border-l-4 border-teal-600 pl-4">
      <h2 class="text-2xl font-semibold mb-1"><a href="{{ post.url | relative_url }}" class="hover:text-teal-600">{{ post.title }}</a></h2>
      <p class="text-sm text-neutral-500 mb-2">{{ post.date | date: "%d %B %Y" }}</p>
      <p class="text-neutral-700 dark:text-neutral-300">{{ post.excerpt | strip_html | truncate: 160 }}</p>
    </article>
    {% endfor %}
  </div>
</section>

---