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

<p v-click class="mie-50">Vous allez voir une capture d'écran d'un site web, un extrait de code, une video, etc, et vous devrez analyser si l'accessibilité est respectée ou pas.</p>

<p v-click class="mie-50">Vous aurez alors 2 réponses possibles : </p>

<div class="flex gap-5 items-center">
    <img v-click alt="" src="/assets/bien-pas-bien.gif" />
    <p v-after class="italic">
        * Attention aux gars qui fume dans le rétro !
    </p>
</div>

---
layout: default
transition: slide-up
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
  :duration="100"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="100" class="text-red-600 text-center font-bold">Le champs de recherche n'a pas de nom accessible (pas de label)</p>

---
layout: default
transition: slide-up
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
  :duration="100"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="100" class="text-[#22BB88] text-center font-bold">Ici l'information est donnée a la fois par le texte en gras, et par un indicateur visuel.</p>

---
layout: default
transition: slide-up
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
  :duration="100"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="100" class="text-red-600 text-center font-bold">Les textes en gris clair ne sont pas suffisament contrastés (2.32:1)</p>


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
  :duration="100"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="100" class="text-red-600 text-center font-bold">L'information est donnée uniquement par la couleur.</p>


---
layout: default
transition: slide-up
---

<h1 class="text-coral font-bold !text-3xl">4. Graphique en camenbert</h1>

<div class="mbs-5 flex justify-center items-center grayscale">
    <img alt="" src="/assets/pie.png" width="600px" />
</div>


<p class="text-red-600 text-center font-bold">L'information est donnée uniquement par la couleur.</p>

<img 
  alt="" 
  src="/assets/Djamel.png" 
  width='50'
  class="absolute end-20 -bottom-8" 
/>


---
layout: default
transition: slide-up
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
  :duration="100"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="100" class="text-red-600 text-center font-bold">L'alternative textuelle est présente mais pas pertinente.</p>


---
layout: default
transition: slide-up
---

<h1 class="text-coral font-bold !text-3xl">6. Bouton "burger"</h1>

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
  :duration="100"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="100" class="text-[#22BB88] text-center font-bold">Le bouton a un nom accessible grâce à l'attribut <code>aria-label</code></p>


---
layout: default
transition: fade
---

<h1 class="text-coral font-bold !text-3xl">7. Video en live</h1>

<div class="mbs-5 flex justify-center items-center">
    <SlidevVideo autoplay controls width="180px">
      <source src="/assets/live-dkt.mp4" type="video/mp4" />
    </SlidevVideo>
</div>

<img 
  alt="" 
  src="/assets/pas-bien.png" 
  width='550'
  class="absolute start-50 top-35" 
  v-click
  v-motion
  :duration="100"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="100" class="text-red-600 text-center font-bold">La video n'est pas sous-titrée, mais...</p>

---
layout: default
transition: slide-up
---

<h1 class="text-coral font-bold !text-3xl">7. Video en live</h1>

<div class="mis-40 mbs-5 flex gap-20 justify-center items-center">
    <SlidevVideo controls width="180px">
      <source src="/assets/live-dkt.mp4" type="video/mp4" />
    </SlidevVideo>
   <div class="flex flex-col">
    <p>Ici il s'agit d'une video live, il est donc difficile et coûteux de sous-titrer ou de proposer une alternative en LSF.</p>
    <p class="font-bold">Il est possible de demander une <br/><a class="text-coral" target="_blank" href="https://accessibilite.numerique.gouv.fr/obligations/champ-application/">"Dérogation pour charge disproportionnée"</a></p>
    <p>En revanche, si la vidéo a vocation à rester sur le site apres sa diffusion initiale, alors il faudra la sous-titrer.</p>
  </div>
</div>


---
layout: default
transition: slide-up
---

<h1 class="text-coral font-bold !text-3xl">8. Facile...</h1>

<div class="mbs-5 flex justify-center items-center">
    <img alt="" src="/assets/west-forever.png" width="650px" />
</div>

<img 
  alt="" 
  src="/assets/pas-bien.png" 
  width='550'
  class="absolute start-50 top-35" 
  v-click
  v-motion
  :duration="100"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="100" class="text-red-600 text-center font-bold">Le texte en blanc sur l'image est illisible</p>


---
layout: default
transition: slide-up
---

<h1 class="text-coral font-bold !text-3xl">9. Renault Twingo</h1>

<div class="mbs-5 flex justify-center items-center">
    <SlidevVideo autoplay controls loop width="850px">
      <source src="/assets/twingo.mov" type="video/mp4" />
    </SlidevVideo>
</div>

<img 
  alt="" 
  src="/assets/pas-bien.png" 
  width='550'
  class="absolute start-50 top-35" 
  v-click
  v-motion
  :duration="100"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="100" class="text-red-600 text-center font-bold">Les animations sont déclenchées au scroll, et on ne peux pas les désactiver</p>


---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-3xl">10. Le meilleur pour la fin !</h1>

<div class="mbs-5 flex justify-center items-center">
    <img alt="" src="/assets/lollipops.png" width="900px" />
</div>

<img 
  alt="" 
  src="/assets/pas-bien.png" 
  width='550'
  class="absolute start-50 top-35" 
  v-click
  v-motion
  :duration="100"
  :initial="{ scale: 1.5, opacity: 0 }"
  :enter="{ scale: 1, opacity: 1 }"
/>

<p v-after 
  :delay="100" class="text-red-600 text-center font-bold">Ici, rien ne va ! <br/>mise en page en tableau, hierarchie des titres, absence de alt, des bouttons à la place des liens, etc, etc...</p>






