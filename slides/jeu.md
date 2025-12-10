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

<!-- 
1. Contraste de couleur
2. Alternatives textuelles
3. Hierarchie des Titres et balise title
4. Les Liens d'évitements
5. Focus visible, et navigation au clavier (sans souris)
6. Sémantique HTML
7. Info évidente (forme, couleur, etc.)
8. Nom accessible (label buttons, label de formulaire, etc.)
-->

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">1. Les contrastes de couleur</h1>

<p class="text-xl">On parle de contraste entre la couleur d'un texte ou d'un élément interactif et la couleur de fond.</p>

<p v-click>Le non-respect du contraste rend le contenu difficile, voire impossible, à lire et exclut une grande partie des utilisateurs malvoyants ou daltoniens.</p>

<p v-click>Les WCAG exigent un ratio minimum de 4.5:1 pour le texte normal et 3:1 pour les éléments interactifs :</p>


<div class="grid grid-cols-2 gap-y-10 mbs-10">
  <div v-click class="is-full flex flex-col gap-2 items-center">
    <p class="text-[#ccc] m-0!">Ce texte n'est pas accesible</p>
    <p class="text-[#333] m-0!">Ce texte est accesible</p>
  </div>

  <div v-click class="is-full flex flex-col gap-4 items-center">
    <button class="px-3 py-1 rounded-md text-white bg-red-100">Ce bouton n'est pas accessible</button>
    <button class="px-3 py-1 rounded-md text-white bg-red-600">Ce bouton est accessible</button>
  </div>

  <div v-click class="is-full flex flex-col gap-1 items-center">
    <label for="input-1">Ce champs n'est pas accessible</label>
    <input id="input-1" class="px-3 py-1 rounded-md text-white border border-[#ddd]"  />
    <label for="input-2">Ce champs est accessible</label>
    <input id="input-2" class="px-3 py-1 rounded-md text-white border border-[#333]"  />
  </div>

  <div v-click class="is-full flex flex-col gap-2 items-center">
    <p class="m-0!">Cette barre de progression n'est pas accessible</p>
    <div class="relative bg-slate-200 w-full h-[20px]">
      <div class="absolute inset-y-0 w-[30%] bg-slate-300 text-white text-xs text-center leading-[20px]">30%</div>
    </div>
    <p class="m-0!">Cette barre de progression est accessible</p>
    <div class="relative bg-slate-400 w-full h-[20px]">
      <div class="absolute inset-y-0 w-[30%] bg-slate-900 text-white text-xs text-center leading-[20px]">30%</div>
    </div>
  </div>
</div>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">2. Les alternatives textuelles</h1>

<p class="text-xl">Certains éléments de la page comme des photos, des videos, des graphiques, des tableaux complexes, etc. peuvent être difficile voire impossible à comprendre pour certaines personnes.</p>

<ul class="mx-10 mbs-5 flex flex-col gap-2">
  <li v-click>
    <strong>Pour les images : </strong>
    <span>Une description de l'image dans l'attribut <code>alt</code> de la balise <code>img</code> (vide si l'image est décorative !)</span>
  </li>

  <li v-click>
    <strong>Pour les videos : </strong>
    <span>Des sous titres (synchronisés) ou éventuellement une transciption textuelle.</span>
  </li>

  <li v-click>
    <strong>Pour les tableaux de données complexes : </strong>
    <span>Via la balise <code>summary</code> de la balise <code>table</code>, ou une balise <code>caption</code>.</span>
  </li>

  <li v-click>
    <strong>Pour les infographies : </strong>
    <span>Une description de l'image dans l'attribut <code>alt</code> si on utilise une image, ou une balise <code>figcaption</code> dans une balise <code>figure</code>.</span>
  </li>
</ul>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">3. Les titres</h1>

<p class="text-xl">L'utilisation de balise de titre permet de structurer l'information dans la page.</p>

<p v-click>Une structure de titre logique est cohérente permet une bonne compréhension de la page et facilite l'accès au différentes sections. Les lecteurs d'écran utilisent les titres pour créer une "Table des matières" de la page.</p>

<div class="grid grid-cols-2 items-center gap-10" >
  <div v-click class="flex flex-col gap-1">
    <div class="font-bold text-sm mis-5">1. DOUDOUNE VESTE JR ADIDAS NOIR</div>
    <div class="font-bold text-sm mis-10">2. Photos du produit</div>
    <div class="font-bold text-sm mis-10">2. Caractéristiques du produit</div>
    <div class="font-bold text-sm mis-10">2. Produits similaires</div>
    <div class="font-bold text-sm mis-15">3. VESTE ENFANT PUMA</div>
    <div class="font-bold text-sm mis-15">3. SWEAT A CAPUCHE UMBRO</div>
    <div class="font-bold text-sm mis-15">3. PARKA NIKE</div>
    <div class="font-bold text-sm mis-10">2. Le produit en vidéo</div>
    <div class="font-bold text-sm mis-10">2. Avis client</div>
    <div class="font-bold text-sm mis-10">2. Pied de page</div>
    <div class="font-bold text-sm mis-15">3. Mentions légales</div>
    <div class="font-bold text-sm mis-15">3. Compte client</div>
  </div>

  <blockquote v-click>
    le style CSS des titres n'est pas forcément lié au niveau de titre de la balise !
  </blockquote>
</div>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">3. La balise title</h1>

<p class="text-xl">C'est elle qui détermine le titre de la page dans l'onglet du navigateur !</p>

<p v-click>C'est également la première chose qui est lue par les lecteurs d'écran au chargement de la page. Le contenu de la balise <code>title</code> doit refléter le contenu de la page, et idéalement contenir le nom du site.</p>

<ul class="grid grid-cols-[1fr_3fr] gap-2 mbs-10">
  <b class="text-end text-red-600" v-click>Mauvais exemples :</b>
  <code v-after>&lt;title&gt;DECATHLON&lt;/title&gt;</code>
  <b class="text-end text-red-600" v-click></b>
  <code v-after>&lt;title&gt;DECATHLON - A fond la forme !&lt;/title&gt;</code>
</ul>

<ul class="grid grid-cols-[1fr_3fr] gap-2 mbs-10">
  <b class="text-end text-[#33CC99]" v-click>Bons exemples :</b>
  <code v-after>&lt;title&gt;DECATHLON - Accueil&lt;/title&gt;</code>
  <b class="text-end text-[#33CC99]" v-click></b>
  <code v-after>&lt;title&gt;DECATHLON - Mon Compte Client&lt;/title&gt;</code>
  <b class="text-end text-[#33CC99]" v-click></b>
  <code v-after>&lt;title&gt;DECATHLON - DOUDOUNE VESTE JR ADIDAS NOIR&lt;/title&gt;</code>
</ul>

<img
  alt="" 
  width="60"
  src="/assets/Arny.png" 
  class="absolute start-10 -bottom-7" 
/>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">4. Les liens d'évitement</h1>

<p>Accéder rapidement aux principales sections de la page</p>

<p v-click>Lorsqu'on navigue sur un site, on consulte plusieurs page. À chaque chargement, le lecteur d'écran reprends la lecture en haut de la page, ce qui peut-être répétitif !</p>

<p v-click>les liens d'évitement permettent d'accéder directement au contenu principal, au menu ou encore au pied de page, en un clique.</p>

<p v-after>Ils réduisent la frustration et le temps passé à naviguer, offrant une expérience utilisateur beaucoup plus efficace pour ceux qui ne peuvent pas utiliser la souris.</p>

<a v-click href="https://www.leroymerlin.fr/" target="_blank" class="text-coral text-3xl mbs-10 inline-block">Exemple</a>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">5. La navigation sans souris</h1>

<p>Certaines personnes ne peuvent pas utiliser une souris pour naviguer, il faut proposer des alternatives.</p>

<p v-click>lorsqu'on navigue au clavier, on a besoin de savoir précisément sur quelle élément de la page on interagit.</p>

<p v-click>Pour cela il faut rendre visible le focus de l'élément.</p>

<div v-after class="mx-50 mbs-15 flex gap-4 justify-center">
  <button class="block w-full outline-offset-4 outline-coral px-6 py-2 rounded-md text-white bg-coral">Ajouter au panier</button>
  <button class="block w-full outline-offset-4 outline-coral px-6 py-2 rounded-md text-white bg-slate-600">Voir mon panier</button>
</div>

<div v-after class="mx-50 mbs-5 flex flex-col gap-1 justify-center">
  <label for="input-5768" class="cursor-pointer">S'abonner à la newsletter</label>
  <input id="input-5768" type="text" class="outline-offset-4 outline-coral px-6 py-2 rounded-md border-2 border-slate-800"/>
</div>

<div v-after class="mx-50 mbs-5 flex gap-1 justify-start">
  <input id="input-5767" type="checkbox" class="relative appearance-none size-6 marker-coral outline-offset-4 outline-coral rounded-md border-2 border-slate-800 checked:after:content-['✓'] after:absolute after:top-[-10px] after:text-coral after-text-3xl"/> 
  <label for="input-5767" class="cursor-pointer">J'accepte les conditions</label>
</div>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">6. la sémantique HTML</h1>

<p>Les balises HTML sont bien faites et en principe accessibles. Il en existe plus d'une centaine pour tous les usages.</p>

<p v-click>Plus le code sera sémantiquement correcte, plus la page sera comprise et interprétée par les lecteurs d'écran, et donc par les utilisateur en situation de handicap visuel.</p>

<p v-click class="mbe-0!">Quelques exemples :</p>

<div class="flex gap-5 items-end">

<div v-click class="mbs-3 flex">
```html
<!-- Une balise mal utilisée -->
<a role="button" href="#" onclick="...">
  Ajouter au panier
</a> 

<button onclick="...">Ajouter au panier</a>
```
</div>

<div v-click class="mbs-3 flex">
```html
<!-- Une image porteuse d'information en CSS -->
<div class="image" style="background-image: url(/img.jpg)"/> 

<img class="image" src="/img.jpg" alt="lorem ipsum..."/>
```
</div>

</div>

<div class="flex gap-5">
<div v-click class="mbs-3 flex">
```html
<!-- Trop de div, aucune structure de page -->
<div class="header">...</div> 
<div class="content">...</div> 
<div class="footer">...</div> 

<header class="header">...</header> 
<main class="content">...</main> 
<footer class="footer">...</footer> 
```
</div>


<div v-click class="mbs-3 flex">
```html
<!-- Du texte dans des div -->
<div>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
</div> 

<p>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
</p> 
```
</div>

</div>

---
layout: default
transition: slide-left
---

<h1 class="text-coral font-bold !text-5xl">7. Évidence de l'information</h1>

<p>Certaines personnes ont des raisonnements différents ou un handicap qui ne leur permet pas de comprendre une information comme tout le monde.</p>

<p v-click class="mbe-0!">Quelques exemples :</p>

<ul class="mis-10 mbs-5 flex flex-col gap-3">
  <li v-click>
    <p class="flex flex-col gap-0 m-0!">
      <b>Les liens dans un paragraphe de texte</b>
      Ils doivent clairement de distinguer clairement, et pas uniquement par la couleur.
    </p>
  </li>

  <li v-click>
    <p class="flex flex-col gap-0 m-0!">
      <b>Les messages d'erreur dans les formulaire</b>
      Il faut indiquer quel champs est en erreur et pourquoi.
    </p>
  </li>

  <li v-click>
    <p class="flex flex-col gap-0 m-0!">
      <b>L'élément actif dans un menu de navigation</b>
      Changer la couleur du lien ou sa forme (en gras par exemple) ne suffit pas.
    </p>
  </li>

  <li v-click>
    <p class="flex flex-col gap-0 m-0!">
      <b>Les message d'alerte</b>
      Précisez si il s'agit d'un mesage d'erreur, d'information, de succès, etc.
    </p>
  </li>

  <li v-click>
    <p class="flex flex-col gap-0 m-0!">
      <b>Les graphiques</b>
      La couleur ne suffit pas pour distinguer les differents segments, il faut une texture ou des annotations
    </p>
  </li>

</ul>

---
layout: default
transition: slide-up
---

<h1 class="text-coral font-bold !text-5xl">8. Les noms accessibles</h1>

<p>Chaque élément interactif de la page doit avoir un nom accesible, c'est à dire un nom qui sera lu par les lecteurs d'écran lors de la prise de focus.</p>


<p v-click>L'exemple le plus courant c'est les boutons représentés par un pictograme.</p>

<p v-after>Même si on est capable de déduire la fonction du button par habitude, les lecteurs d'écran eux, en sont incapables. Ils diront simplement "Bouton".</p>

<div v-click class="mbs-1 flex">
```html
<!-- Ici on ne sait pas à quoi sert le bouton -->
<button onClick={login} class="login-btn">
  <Icon name="user" />
</button>
```
</div>

<div v-click class="mbs-1 flex">
```html
<button onClick={login} class="login-btn" aria-label="Se connecter à l'espace client">
  <Icon name="user" />
</button>
```
</div>

<div v-click class="mbs-1 flex">
```html
<button onClick={login} class="login-btn">
  <span class="sr-only">Se connecter à l'espace client</span>
  <Icon name="user" />
</button>
```
</div>

