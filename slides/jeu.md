---
layout: center
transition: fade
---

<h1 class="text-coral font-bold !text-7xl">Une équipe en OR</h1>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">Une équipe en OR.</h1>

<p class="text-2xl">Connaissez-vous les points les plus importants en A11Y ?</p>

<p v-click class="mbs-10">Il existe des points clés en accessibilité qui, lorsqu’ils sont bien appliqués, garantissent un site largement utilisable par tout le monde.</p>

<p v-click>Nous en avons listé 8, à vous de les trouver ! </p>

<a v-after class="inline-block mbs-20 text-coral text-3xl font-semibold" href="https://cv.basileparent.fr/accessible-family-feud/" target="_blank">Lancer le jeu !</a>

<img 
  alt="" 
  src="/assets/feud.png" 
  width='550'
  class="absolute end-0 bottom-0" 
  v-after
  v-motion
  :delay="125"
  :duration="500"
  :initial="{ x: 600 }"
  :enter="{ x: 0 }"
/>
