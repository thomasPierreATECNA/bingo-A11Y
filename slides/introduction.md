---
layout: default
transition: slide-up
---

<h1 class="text-coral font-bold !text-5xl">Introduction.</h1>

<p class="text-2xl">Mais d'abord c'est quoi l'accessibilité numérique ?</p>


<div class="mbs-10 max-w-[65%] text-2xl!">
  <blockquote v-click class="text-2xl! p-5!">
    C'est concevoir des interfaces compréhensibles, perceptibles et utilisables par <u>tous</u>. 
    <br/>
    Y compris les personnes en situation de handicap.
  </blockquote>

  <img 
  alt="" 
  src="/assets/dev-3.png" 
  class="absolute end-20 bottom-0" 
  v-after
  v-motion
    :delay="125"
    :duration="250"
    :initial="{ x: 350 }"
    :enter="{ x: 0 }"
  />

  <p v-click class="mbs-20! text-center text-4xl!">Autrement dit, tout le monde est concerné !</p>
</div>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">les grands types de handicap</h1>

<p class="text-2xl">Il existe 5 grands types de handicap : </p>

<ul class="mbs-10">
  <li v-click><strong>le handicap moteur: </strong> (difficulté de mouvement, paralysie, amputation, etc.)</li>
  <li v-click><strong>le handicap sensoriel: </strong> (cécité ou surdité, totale ou partielle)</li>
  <li v-click><strong>le handicap mental: </strong> (Déficience intellectuelle légère, modérée ou sévère)</li>
  <li v-click><strong>le handicap psychique: </strong> (Schizophrénie, bipolarité, dépression, TOC, etc.)</li>
  <li v-click><strong>le handicap cognitif: </strong> (troubles DYS, autisme, TDA, etc.)</li>
</ul>

<blockquote v-click class="mbs-10 mx-20">
  <h2 class="text-xl! mbe-3! font-semibold"><uim-rocket class="text-sky-900"/> Bon à savoir !</h2>
  <p class="text-lg text-slate-800">Un handicap peut-être permanent ou provisoire.</p>
  <p class="text-lg text-slate-800">On peux se retrouver dans une situation de handicap provisoire comme un bras dans le plâtre, un environement bruyant, un ecran de téléphone brisé, etc.</p>
</blockquote>

---
layout: default
transition: slide-left
---

<div class="flex flex-col gap-10 items-start text-start max-w-[60%] mis-auto">
  <h1 class="text-coral font-bold !text-5xl">Question !</h1>
  <p class="text-2xl">Combien de personnes<br/>en situation de handicap en France selon vous ? </p>

  <img alt="" src="/assets/dev-6.png" class="absolute start-20 bottom-0"/>

  <p v-click class="text-3xl text-coral font-semibold">Entre 7 et 12 Millions selon les sources </p>
  <ul class="flex flex-col gap-4">
    <li v-click class="text-lg leading-[1.25]! text-start text-slate-600">Plus de 3,1 millions de personnes disposent d'une reconnaissance administrative de leur handicap</li>
    <li v-click class="text-lg leading-[1.25]! text-start text-slate-600">Environ 1,29 million de personnes reçoivent l'Allocation aux Adultes Handicapés (AAH)</li>
  </ul>
</div>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">Les réferentiels</h1>

<p class="text-xl">Pour garantir et mesurer l'A11Y, on s'appui sur des référentiels fondamentaux : </p>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">Les WCAG <small class="text-xl">(Web Content Accessibility Guidelines)</small></h1>

<p class="text-xl">C'est le référentiel international.</p>

<p v-click class="text-xl">Les WCAG sont les directives universelles publiées par le <a class="text-coral" href="https://www.w3.org/WAI/standards-guidelines/wcag/fr">W3C (World Wide Web Consortium)</a>. Elles constituent la base technique de la quasi-totalité des lois et référentiels d'accessibilité dans le monde.</p>

<p v-click class="text-xl">Les WCAG sont structurées autour de quatre principes majeurs (POUR)</p>

<ul class="flex flex-col gap-5 mie-50">
  <li v-click class="leading-[1.25]!">
    <strong>Perceptible</strong>: L'information doit être présentée de manière à être perceptible par tous les sens (ex: alternatives textuelles pour les images).
  </li>

  <li v-click class="leading-[1.25]!">
    <strong>Utilisable</strong>: Les composants d'interface et la navigation doivent être utilisables (ex: accessibilité au clavier, temps suffisant pour interagir).
  </li>

  <li v-click class="leading-[1.25]!">
    <strong>Compréhensible</strong>: L'information et l'utilisation de l'interface doivent être compréhensibles (ex: texte lisible, prédictibilité des interactions).
  </li>

  <li v-click class="leading-[1.25]!">
    <strong>Robuste</strong>: Le contenu doit pouvoir être interprété par une grande variété d'agents utilisateurs, y compris les technologies d'assistance (ex: balises sémantiques correctes).
  </li>
</ul>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">Les WCAG <small class="text-xl">(Web Content Accessibility Guidelines)</small></h1>

<p class="text-xl">Les critères de succès des WCAG sont classés en trois niveaux de conformité :</p>

<ul class="flex flex-col gap-5 mie-50 mbs-20!">
  <li v-click class="leading-[1.25]!">
    <strong>A (Minimum)</strong>: Le niveau de base, essentiel pour que la majorité des utilisateurs puissent accéder au contenu.
  </li>

  <li v-click class="leading-[1.25]!">
    <strong>AA (Cible)</strong>: Le niveau le plus couramment recommandé et souvent exigé par la loi dans le monde (dont l'Union Européenne et la France). Il permet l'accessibilité à la grande majorité des technologies d'assistance.
  </li>

  <li v-click class="leading-[1.25]!">
    <strong>AAA (Optimal)</strong>: Le plus haut niveau d'accessibilité, généralement difficile à atteindre pour l'ensemble d'un site.
  </li>
</ul>

<p v-click class="font-italic mbs-10! text-center">(La version actuelle courante est WCAG 2.1, avec la version 2.2 et 3.0 en cours de déploiement.)</p>


---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">Le RGAA <small class="text-xl">(Référentiel Général d'Amélioration de l'Accessibilité)</small></h1>

<p class="text-xl">C'est le référentiel Français.</p>

<p v-click class="text-xl">Le RGAA est l'application concrète des WCAG dans le contexte légal français. C'est la norme officielle à laquelle doivent se conformer les organismes publics et certaines entreprises privées en France (Loi de 2005 et décret de 2019).</p>

<p v-click class="text-xl">Il se compose de <a href="https://accessibilite.numerique.gouv.fr/methode/criteres-et-tests/" class="text-coral">106 critères répartis en 13 thématiques</a>.</p>



<blockquote v-click class="mbs-20 mx-40">
  <h2 class="text-xl! mbe-3! font-semibold"><uim-rocket class="text-sky-900"/> Important !</h2>
  <p class="text-lg text-slate-800">Pour qu'un critère soit considéré comme conforme, il faut qu'il le soit sur la totalité des pages de l'échantillon.</p>
</blockquote>