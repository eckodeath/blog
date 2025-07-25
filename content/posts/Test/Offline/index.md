---
title: "Test en cours"
date: 2025-07-20
draft: false
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


### Une seule photo plus large que le texte :

<div class="medium-wide-image">
  <img src="/posts/test/offline/iphone_16_unboxing_1.jpg" alt="Image un peu plus large que le texte" />
</div>



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

