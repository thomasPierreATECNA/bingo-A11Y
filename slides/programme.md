---
layout: default
transition: slide-left
---

<h1 class="!text-6xl text-coral font-bold">Au programme</h1>

<ol class="font-bold text-3xl text-slate-700 mbs-30 mis-10">
  <li>Introduction</li>
  <li>Une équipe en Or </li>
  <li>Le code de l'Accessibilité</li>
</ol>

<img 
  alt="" 
  src="/assets/dev-1.png" 
  class="absolute end-20 bottom-0" 
  v-motion
  :delay="125"
  :duration="250"
  :initial="{ x: 350 }"
  :enter="{ x: 0 }"
/>