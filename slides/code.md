---
layout: center
transition: fade
---

<h1 class="text-coral font-bold !text-7xl">Le code de l'accessibilité</h1>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">Le code de l'accessibilité</h1>

<p class="text-2xl">Le principe est très simple !</p>

<p v-click class="mie-50">Vous allez voir une capture d'écran d'un site web, un extrait de code, une video, etc, et vous devrez analyser si l'accesibilité est respectée ou pas.</p>

<p v-click class="mie-50">Vous aurez alors 2 réponses possibles : </p>

<div class="flex gap-5 items-center">
    <img v-click alt="" src="/assets/bien-pas-bien.gif" />
    <p v-after class="italic">
        * Attention aux gars qui fume dans le rétro !
    </p>
</div>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-3xl">1. Moteur de recherche</h1>

<div class="mbs-5 flex justify-center items-center">
    <img alt="" src="/assets/no-label-input.png" width="800px" />
</div>

<img 
  alt="" 
  src="/assets/pas-bien.png" 
  width='550'
  class="absolute start-50 top-35" 
  v-click
  v-motion
  :duration="300"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="300" class="text-red-600 text-center font-bold">Les champs du formulaire n'ont pas de nom accessible (pas de label)</p>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-3xl">2. Élement actif du menu</h1>

<div class="mbs-5 flex justify-center items-center">
    <img alt="" src="/assets/lien-courrant.png" width="800px" />
</div>

<img 
  alt="" 
  src="/assets/bien.png" 
  width='550'
  class="absolute start-50 top-35" 
  v-click
  v-motion
  :duration="300"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="300" class="text-[#22BB88] text-center font-bold">Ici l'information est donnée a la fois par le texte en gras, et par un indicateur visuel.</p>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-3xl">3. Les membres de l'équipe</h1>

<div class="mbs-5 flex justify-center items-center">
    <img alt="" src="/assets/contrast.png" width="750px" />
</div>

<img 
  alt="" 
  src="/assets/pas-bien.png" 
  width='550'
  class="absolute start-50 top-35" 
  v-click
  v-motion
  :duration="300"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="300" class="text-red-600 text-center font-bold">Le texte en gris clair ne sont pas suffisament contrastés (2.32:1)</p>


---
layout: default
transition: fade
---

<h1 class="text-coral font-bold !text-3xl">4. Graphique en camenbert</h1>

<div class="mbs-5 flex justify-center items-center">
    <img alt="" src="/assets/pie.png" width="600px" />
</div>

<img 
  alt="" 
  src="/assets/pas-bien.png" 
  width='550'
  class="absolute start-50 top-35" 
  v-click
  v-motion
  :duration="300"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="300" class="text-red-600 text-center font-bold">L'indication par la couleur n'est pas suffisante.</p>


---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-3xl">4. Graphique en camenbert</h1>

<div class="mbs-5 flex justify-center items-center grayscale">
    <img alt="" src="/assets/pie.png" width="600px" />
</div>


<p v-after 
  :delay="300" class="text-red-600 text-center font-bold">L'indication par la couleur n'est pas suffisante.</p>


---
layout: default
transition: fade
---

<h1 class="text-coral font-bold !text-3xl">5. Alternative textuelle</h1>

<div class="mbs-5 flex justify-center items-center">
    <img alt="" src="/assets/score.png" width="800px" />
</div>

<img 
  alt="" 
  src="/assets/pas-bien.png" 
  width='550'
  class="absolute start-50 top-35" 
  v-click
  v-motion
  :duration="300"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="300" class="text-red-600 text-center font-bold">L'alternative textuelle est présente mais pas pertinente.</p>


---
layout: default
transition: fade
---

<h1 class="text-coral font-bold !text-3xl">6. Boutton "burger"</h1>

<div class="mbs-5 flex justify-center items-center">
    <img alt="" src="/assets/apple.png" width="800px" />
</div>

<img 
  alt="" 
  src="/assets/bien.png" 
  width='550'
  class="absolute start-50 top-35" 
  v-click
  v-motion
  :duration="300"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="300" class="text-[#22BB88] text-center font-bold">Le bouton a un nom accessible grâce à l'attribut <code>aria-label</code></p>


---
layout: default
transition: fade
---

<h1 class="text-coral font-bold !text-3xl">7. Video en live"</h1>

<div class="mbs-5 flex justify-center items-center">
    <SlidevVideo v-click autoplay controls width="180px">
    <source src="/assets/live-dkt.mp4" type="video/mp4" />
    <p>
        Your browser does not support videos. You may download it
        <a href="/assets/live-dkt.mp4">here</a>.
    </p>
    </SlidevVideo>
</div>

<img 
  alt="" 
  src="/assets/pas-bien.png" 
  width='550'
  class="absolute start-50 top-35" 
  v-click
  v-motion
  :duration="300"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="300" class="text-red-600 text-center font-bold">La video n'est pas sous-titrée</p>



