---
title: "Test en cours"
date: 2025-04-20
draft: true
tags: ["blog", "écriture", "indépendance", "hugo", "github", "netlify"]
categories: ["Journal"]
summary: "Ceci est un article test afin de tester les nouvelles implantations"
cover:
    image: "/posts/test/offline/cover_3.jpg"
    alt: ""
    caption: ""
    relative: false
---

Ceci est une page test - pensez à mettre le fichier en draft à la fin

### Galerie carré pour photos qui ne sont pas de la même taille :

<div class="medium-wide-image">
  <div class="image-grid">
    <figure>
      <img src="/posts/test/offline/iphone_16_unboxing_1.jpg" alt="Photo 1">
    </figure>
    <figure>
      <img src="/posts/voyages/norway-part-1/Norway_Part_1_Blog_6-min.jpg" alt="Photo 2">
    </figure>
    <figure>
      <img src="/posts/test/offline/iphone_16_unboxing_3.jpg" alt="Photo 3">
    </figure>
    <figure>
      <img src="/posts/voyages/norway-part-1/Norway_Part_1_Blog_5-min.jpg" alt="Photo 4">
    </figure>
  </div>
</div>

------

### Galerie carré pour photos qui font la même taille :

<div class="medium-wide-image">
  <div class="side-by-side">
    <figure>
      <img src="/posts/test/offline/iphone_16_unboxing_1.jpg" alt="Photo 1">
    </figure>
    <figure>
      <img src="/posts/test/offline/iphone_16_unboxing_2.jpg" alt="Photo 2">
    </figure>
    <figure>
      <img src="/posts/test/offline/iphone_16_unboxing_3.jpg" alt="Photo 3">
    </figure>
    <figure>
      <img src="/posts/test/offline/iphone_16_unboxing_4.jpg" alt="Photo 4">
    </figure>
  </div>
</div>

------

### Une seule photo plus large que le texte :

<div class="medium-wide-image">
  <img src="/posts/test/offline/iphone_16_unboxing_1.jpg" alt="Image un peu plus large que le texte" />
</div>

------

### Une seule photo plus large que le texte avec lien cliquable vers site extérieur :

<div class="medium-wide-image">
  <a href="https://eckodeath.carrd.co" target="_blank" rel="noopener">
    <img src="/images/Carrd_Screen.png" alt="Image un peu plus large que le texte" />
  </a>
</div>

------

### Deux photos verticales (ou pas) plus large que le texte :

<div class="medium-wide-image">
  <div class="side-by-side">
    <figure>
      <img src="/posts/voyages/norway-part-1/Norway_Part_1_Blog_5-min.jpg" alt="Photo 3">
    </figure>
    <figure>
      <img src="/posts/voyages/norway-part-1/Norway_Part_1_Blog_6-min.jpg" alt="Photo 2">
    </figure>
  </div>
</div>

------

### Deux photos une verticale et une horizontale plus large que le texte :

<div class="medium-wide-image side-by-side-ratio">
  <figure class="vertical">
    <img src="/posts/lifestyle/achat-MacBook-Air-M4/MacBook_Air_M4_unboxing_4.jpg" alt="Verticale">
  </figure>
  <figure class="horizontal">
    <img src="/posts/lifestyle/achat-MacBook-Air-M4/MacBook_Air_M4_unboxing_7.jpg" alt="Horizontale">
  </figure>
</div>

------

### Grille de 3 photos :

<div class="medium-wide-image image-grid grid-3">
  <figure>
    <img src="/posts/test/offline/iphone_16_unboxing_4.jpg" alt="Photo 1">
  </figure>
  <figure>
    <img src="/posts/test/offline/iphone_16_unboxing_3.jpg" alt="Photo 2">
  </figure>
  <figure>
    <img src="/posts/test/offline/iphone_16_unboxing_2.jpg" alt="Photo 3">
  </figure>
</div>

------

### Texte à gauche et photo à droite :

<section class="text-left-image-right">
  <div class="text-block">
    <h2>Mon titre accrocheur</h2>
    <p>
    Voici un paragraphe de texte pour présenter une idée, une expérience ou un produit.</p>
    <p>Tu peux y ajouter autant de texte que tu veux.
    </p>
  </div>
  <div class="image-block">
    <img src="/posts/voyages/norway-part-1/Norway_Part_1_Blog_5-min.jpg" alt="Paysage norvégien" />
  </div>
</section>


### Texte à droite et photo à gauche :

<section class="text-left-image-right reverse">
  <div class="text-block">
    <h2>Un autre titre</h2>
    <p>
      Ce texte apparaîtra à droite de l’image sur les grands écrans.
    </p>
  </div>
  <div class="image-block">
    <img src="/posts/voyages/norway-part-1/Norway_Part_1_Blog_5-min.jpg" alt="Image illustrant le texte" />
  </div>
</section>


------

Image seule centré à 80% de sa taille :

<center>
  <img src="/images/Instagram_roadtrip_edito pellicule.png" alt="Description" style="width: 80%;">
</center>


------


### Ancienne version :

{{< gallery >}}

  {{< figure src="/posts/test/offline/iphone_16_unboxing_1.jpg" caption="Photo 1" >}}
  {{< figure src="/posts/test/offline/iphone_16_unboxing_2.jpg" caption="Photo 2" >}}
  {{< figure src="/posts/test/offline/iphone_16_unboxing_3.jpg" caption="Photo 3" >}}
  {{< figure src="/posts/test/offline/iphone_16_unboxing_4.jpg" caption="Photo 4" >}}


{{< /gallery >}}

{{< rawhtml >}}
  <p class="speshal-fancy-custom">
    <div class="medium-wide-image">
  <img src="/posts/test/offline/iphone_16_unboxing_2.jpg" alt="Image un peu plus large que le texte" />
</div>
  </p>
{{< /rawhtml >}}

{{< rawhtml >}}
  <p class="speshal-fancy-custom">
  <div class="side-by-side">
  {{< figure src="/posts/test/offline/iphone_16_unboxing_3.jpg" alt="Photo 3" >}}
  {{< figure src="/posts/test/offline/iphone_16_unboxing_4.jpg" alt="Photo 4" >}}
</div>
  </p>
{{< /rawhtml >}}

{{< rawhtml >}}
  <p class="speshal-fancy-custom">
    <div class="medium-wide-image">
  <div class="side-by-side">
  {{< figure src="/posts/test/offline/iphone_16_unboxing_3.jpg" alt="Photo 3" >}}
  {{< figure src="/posts/test/offline/iphone_16_unboxing_4.jpg" alt="Photo 4" >}}
</div>
  </p>
{{< /rawhtml >}}

### Texte à gauche et photo à droite :

<section class="text-image-section">
  <div class="content">
    <h2>Mon titre accrocheur</h2>
    <p>
      Voici un paragraphe de texte pour présenter une idée, une expérience ou un produit.
      Ce bloc se trouve à gauche, pendant que l’image est à droite.
    </p>
    <p>
      Tu peux y ajouter autant de texte que tu veux. Ce format est idéal pour des pages "À propos", "Projet", ou "Voyage".
    </p>
  </div>
  <div class="image">
    <img src="/posts/voyages/norway-part-1/Norway_Part_1_Blog_5-min.jpg" alt="Photo illustrative" />
  </div>
</section>

<style>
.text-image-section {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: space-between;
  gap: 2rem;
  margin: 2rem 0;
}

.text-image-section .content {
  flex: 1 1 50%;
}

.text-image-section .image {
  flex: 1 1 40%;
}

.text-image-section img {
  max-width: 100%;
  height: auto;
  border-radius: 8px;
}

/* Responsive pour les petits écrans */
@media (max-width: 768px) {
  .text-image-section {
    flex-direction: column;
  }
}
</style>

