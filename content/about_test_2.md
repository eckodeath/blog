---
title: "À propos"
date: 2025-07-28
draft: false
---

<section class="about-hero">
  <div class="about-hero-text">
    <h2 class="about-section-label">Mon histoire</h2>
    <p>Je m'appelle Kurt Grava, j'ai 38 ans et depuis 2012, je publie sous le nom @eckodeath. Eckodeath est un projet personnel né de mes passions pour le voyage, la photographie, le partage d'expériences et la technologie.</p>
    <p>Je suis un blogueur indépendant, un photographe autodidacte et un amoureux du numérique. J'aime capturer ce qui m'entoure, raconter ce que je vis, tester ce qui m'inspire, vivre tout simplement.</p>
    <p>Mon blog est un espace personnel et créatif où je combine images, récits et réflexions, avec pour objectif de partager mes expériences avec sincérité, inspirer celles et ceux qui aiment explorer, créer des connexions autour de passions communes : le voyage, la photographie et la technologie.</p>
    <p class="about-hero-link">→ <a href="https://eckodeath.fr/posts/l_homme_derriere_le_pseudo/" target="_blank">L'homme derrière le pseudo, qui suis-je réellement ?</a></p>
  </div>
  <div class="about-hero-photo">
    <img src="/images/about_profil_2.png" alt="Portrait de Kurt Grava" />
  </div>
</section>

<div class="about-divider"></div>

<section class="about-block">
  <h2 class="about-section-label">Le blog</h2>
  <p>Eckodeath.fr est un site web statique créé avec <a href="https://gohugo.io/" target="_blank">Hugo</a> et j'utilise le thème <a href="https://github.com/adityatelange/hugo-PaperMod" target="_blank">PaperMod</a> pour obtenir un design épuré et responsive. J'ai optimisé le site moi-même et avec beaucoup d'amour et surtout de patience. Le code source est géré sur <a href="https://github.com/" target="_blank">GitHub</a> et le site est déployé automatiquement via <a href="https://www.netlify.com/" target="_blank">Netlify</a>. Le nom de domaine eckodeath.fr est quant à lui enregistré et géré chez <a href="https://www.ovhcloud.com/" target="_blank">OVH</a>.</p>
</section>

<div class="about-divider"></div>

<section class="about-block">
  <h2 class="about-section-label">Mon matériel</h2>
  <p>J'ai décidé de créer une page dédiée afin de vous permettre de découvrir, si vous le souhaitez, l'ensemble du matériel que j'utilise au quotidien. Cette page est mise à jour au fur et à mesure de l'évolution de mon setup.</p>
  <a href="https://eckodeath.fr/materiel/" class="about-cta">Mon matériel au quotidien →</a>
  <p class="about-note">Les liens proposés sur cette page (et sur certaines autres du blog) sont des liens affiliés — cela ne change rien pour vous et vous permet de me soutenir.</p>
</section>

<div class="about-divider"></div>

<section class="about-block">
  <h2 class="about-section-label">Mes réseaux sociaux</h2>
  <p>Merci de suivre mes aventures sur <strong>eckodeath.fr</strong>. Si vous souhaitez me suivre sur les divers réseaux sociaux que j'utilise, retrouvez tous mes liens sur <a href="https://eckodeath.carrd.co" target="_blank">eckodeath.carrd.co</a>.</p>
</section>

<div class="about-divider"></div>

<p class="about-copyright">© eckodeath.fr — Tous droits réservés. Les textes, photos et vidéos partagés ici sont le fruit de mon travail et de mes expériences. Merci de ne pas les utiliser sans mon autorisation écrite. Si vous souhaitez partager un extrait, contactez-moi : je suis toujours ouvert à l'échange.</p>

<style>
.about-hero {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 2rem;
  margin: 2rem 0 2.5rem;
}
.about-hero-photo {
  flex: 1 1 45%;
  text-align: center;
}
.about-hero-photo img {
  max-width: 100%;
  height: auto;
  border-radius: 12px;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.15);
  display: block;
  margin: 0 auto;
}
.about-hero-text {
  flex: 1 1 50%;
  font-size: 15px;
  line-height: 1.7;
}
.about-hero-text p {
  margin-bottom: 1rem;
}
.about-hero-link {
  margin-top: 1.5rem !important;
  font-family: var(--font-mono, 'DM Mono', monospace);
  font-size: 0.85rem !important;
}
.about-section-label {
  font-size: 0.72rem !important;
  font-family: var(--font-mono, 'DM Mono', monospace) !important;
  font-weight: 600 !important;
  letter-spacing: 0.12em !important;
  text-transform: uppercase !important;
  color: var(--secondary) !important;
  margin-bottom: 1.2rem !important;
  border: none !important;
}
.about-divider {
  border-top: 1px solid var(--border);
  margin: 2.5rem 0;
}
.about-block {
  font-size: 15px;
  line-height: 1.7;
}
.about-block p {
  margin-bottom: 1rem;
}
.about-cta {
  display: inline-block;
  margin: 0.5rem 0 1.2rem;
  font-family: var(--font-mono, 'DM Mono', monospace);
  font-size: 0.85rem;
  color: var(--primary);
  text-decoration: none;
  border-bottom: 1px solid var(--primary);
  padding-bottom: 1px;
  transition: opacity 0.2s;
}
.about-cta:hover {
  opacity: 0.6;
}
.about-note {
  font-size: 0.82rem !important;
  color: var(--secondary);
  font-style: italic;
}
.about-copyright {
  font-size: 0.8rem;
  color: var(--secondary);
  line-height: 1.6;
}
@media (max-width: 640px) {
  .about-hero {
    flex-direction: column;
  }
  .about-hero-photo {
    flex: 0 0 auto;
    width: 100%;
    max-width: 280px;
    margin: 0 auto;
  }
}
</style>