---
title: "À propos"
date: 2025-07-28
layout: "single"
hideMeta: true
---

<style>
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=DM+Sans:wght@300;400;500&family=DM+Mono:wght@400;500&display=swap');

  :root {
    --ink: #0f0f0f;
    --cream: #f5f0e8;
    --rust: #c0392b;
    --sand: #d4c5a9;
    --smoke: #8a8279;
    --white: #ffffff;
  }

  .about-wrapper {
    font-family: 'DM Sans', sans-serif;
    max-width: 860px;
    margin: 0 auto;
    color: var(--ink);
    line-height: 1.7;
  }

  /* ─── HERO ─────────────────────────────────────────────── */
  .about-hero {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 0;
    min-height: 380px;
    margin-bottom: 80px;
    position: relative;
  }

  .about-hero__text {
    background: var(--ink);
    color: var(--cream);
    padding: 48px 40px 40px 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    position: relative;
    z-index: 2;
  }

  .about-hero__text::after {
    content: '';
    position: absolute;
    right: -28px;
    top: 0;
    bottom: 0;
    width: 56px;
    background: var(--ink);
    clip-path: polygon(0 0, 0 100%, 100% 50%);
    z-index: 3;
  }

  .about-hero__eyebrow {
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    letter-spacing: 0.25em;
    text-transform: uppercase;
    color: var(--rust);
    margin-bottom: 16px;
  }

  .about-hero__name {
    font-family: 'Playfair Display', serif;
    font-size: clamp(2rem, 5vw, 3.2rem);
    font-weight: 700;
    line-height: 1.1;
    color: var(--white);
    margin: 0 0 12px 0;
  }

  .about-hero__alias {
    font-family: 'DM Mono', monospace;
    font-size: 13px;
    color: var(--sand);
    letter-spacing: 0.1em;
  }

  .about-hero__image {
    position: relative;
    overflow: hidden;
  }

  .about-hero__image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: top center;
    display: block;
    filter: grayscale(20%) contrast(1.05);
  }

  .about-hero__image::before {
    content: '';
    position: absolute;
    inset: 0;
    background: linear-gradient(135deg, transparent 60%, rgba(192,57,43,0.18));
    z-index: 1;
    pointer-events: none;
  }

  /* ─── INTRO QUOTE ────────────────────────────────────────── */
  .about-quote {
    border-left: 3px solid var(--rust);
    margin: 0 0 72px 0;
    padding: 8px 0 8px 28px;
  }

  .about-quote p {
    font-family: 'Playfair Display', serif;
    font-style: italic;
    font-size: clamp(1.1rem, 2.5vw, 1.35rem);
    color: var(--ink);
    margin: 0;
    line-height: 1.6;
  }

  /* ─── SECTION TITLES ─────────────────────────────────────── */
  .about-section {
    margin-bottom: 64px;
  }

  .about-section__label {
    font-family: 'DM Mono', monospace;
    font-size: 10px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: var(--rust);
    display: block;
    margin-bottom: 8px;
  }

  .about-section__title {
    font-family: 'Playfair Display', serif;
    font-size: clamp(1.4rem, 3vw, 1.9rem);
    font-weight: 700;
    margin: 0 0 24px 0;
    color: var(--ink);
    line-height: 1.2;
  }

  .about-section p {
    font-weight: 300;
    font-size: 1rem;
    color: #2a2a2a;
    margin-bottom: 16px;
  }

  /* ─── PILLARS GRID ───────────────────────────────────────── */
  .about-pillars {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1px;
    background: var(--sand);
    margin: 40px 0 72px;
    border: 1px solid var(--sand);
  }

  .pillar {
    background: var(--white);
    padding: 28px 24px;
    text-align: center;
    transition: background 0.25s ease;
  }

  .pillar:hover {
    background: var(--cream);
  }

  .pillar__icon {
    font-size: 1.6rem;
    display: block;
    margin-bottom: 10px;
  }

  .pillar__title {
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--rust);
    display: block;
    margin-bottom: 6px;
  }

  .pillar__text {
    font-size: 0.85rem;
    font-weight: 300;
    color: var(--smoke);
    margin: 0;
  }

  /* ─── TECH STACK ─────────────────────────────────────────── */
  .about-stack {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 20px;
  }

  .stack-tag {
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    letter-spacing: 0.08em;
    padding: 6px 14px;
    border: 1px solid var(--sand);
    color: var(--smoke);
    background: transparent;
    transition: all 0.2s ease;
    text-decoration: none;
    display: inline-block;
  }

  .stack-tag:hover {
    border-color: var(--rust);
    color: var(--rust);
    background: var(--cream);
    text-decoration: none;
  }

  /* ─── DIVIDER ────────────────────────────────────────────── */
  .about-rule {
    border: none;
    height: 1px;
    background: linear-gradient(to right, var(--rust), var(--sand), transparent);
    margin: 0 0 64px;
  }

  /* ─── CTA ROW ────────────────────────────────────────────── */
  .about-cta-row {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
    margin-top: 28px;
  }

  .about-cta {
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    padding: 12px 24px;
    text-decoration: none;
    transition: all 0.2s ease;
    display: inline-block;
  }

  .about-cta--primary {
    background: var(--ink);
    color: var(--cream);
    border: 2px solid var(--ink);
  }

  .about-cta--primary:hover {
    background: var(--rust);
    border-color: var(--rust);
    color: var(--white);
    text-decoration: none;
  }

  .about-cta--secondary {
    background: transparent;
    color: var(--ink);
    border: 2px solid var(--sand);
  }

  .about-cta--secondary:hover {
    border-color: var(--ink);
    text-decoration: none;
  }

  /* ─── FOOTER NOTE ────────────────────────────────────────── */
  .about-footer-note {
    margin-top: 80px;
    padding: 28px 32px;
    background: var(--cream);
    border-left: 3px solid var(--sand);
    font-size: 0.85rem;
    font-weight: 300;
    color: var(--smoke);
  }

  .about-footer-note strong {
    color: var(--ink);
    font-weight: 500;
  }

  /* ─── RESPONSIVE ─────────────────────────────────────────── */
  @media (max-width: 640px) {
    .about-hero {
      grid-template-columns: 1fr;
      min-height: auto;
    }

    .about-hero__text {
      padding: 36px 24px 36px 24px;
    }

    .about-hero__text::after {
      display: none;
    }

    .about-hero__image {
      height: 260px;
    }

    .about-pillars {
      grid-template-columns: 1fr;
    }

    .about-cta-row {
      flex-direction: column;
    }
  }
</style>

<div class="about-wrapper">

  <!-- HERO -->
  <div class="about-hero">
    <div class="about-hero__text">
      <span class="about-hero__eyebrow">// depuis 2012</span>
      <h1 class="about-hero__name">Kurt<br>Grava</h1>
      <span class="about-hero__alias">@eckodeath</span>
    </div>
    <div class="about-hero__image">
      <img src="/images/about_profil_2.png" alt="Portrait de Kurt Grava" loading="lazy">
    </div>
  </div>

  <!-- INTRO QUOTE -->
  <blockquote class="about-quote">
    <p>Blogueur indépendant, photographe autodidacte<br>
    et amoureux du numérique — j'aime capturer ce qui m'entoure,<br>
    raconter ce que je vis, tester ce qui m'inspire.</p>
  </blockquote>

  <!-- SECTION : MON HISTOIRE -->
  <section class="about-section">
    <span class="about-section__label">01 — Qui suis-je</span>
    <h2 class="about-section__title">Mon histoire</h2>
    <p>
      Je m'appelle Kurt Grava, j'ai 38 ans et depuis 2012, je publie sous le nom
      <strong>@eckodeath</strong>. Ce projet personnel est né de mes passions pour le voyage,
      la photographie, le partage d'expériences et la technologie.
    </p>
    <p>
      Mon blog est un espace créatif où je combine images, récits et réflexions,
      avec pour objectif de partager mes expériences avec sincérité, d'inspirer
      celles et ceux qui aiment explorer, et de créer des connexions autour de
      passions communes.
    </p>
    <div class="about-cta-row">
      <a href="https://eckodeath.fr/posts/lhomme-derriere-le-pseudo/" class="about-cta about-cta--primary">
        L'homme derrière le pseudo →
      </a>
    </div>
  </section>

  <!-- PILLARS -->
  <div class="about-pillars">
    <div class="pillar">
      <span class="pillar__icon">✈️</span>
      <span class="pillar__title">Voyage</span>
      <p class="pillar__text">Explorer, s'émerveiller, raconter.</p>
    </div>
    <div class="pillar">
      <span class="pillar__icon">📷</span>
      <span class="pillar__title">Photo</span>
      <p class="pillar__text">Capturer l'instant, figer la lumière.</p>
    </div>
    <div class="pillar">
      <span class="pillar__icon">💻</span>
      <span class="pillar__title">Technologie</span>
      <p class="pillar__text">Tester, apprendre, partager.</p>
    </div>
  </div>

  <hr class="about-rule">

  <!-- SECTION : LE BLOG -->
  <section class="about-section">
    <span class="about-section__label">02 — La technique</span>
    <h2 class="about-section__title">Le blog</h2>
    <p>
      Eckodeath.fr est un site statique construit avec <strong>Hugo</strong> et le thème
      <strong>PaperMod</strong> pour un design épuré et responsive. Le code source vit sur
      <strong>GitHub</strong>, le déploiement est automatisé via <strong>Netlify</strong>,
      et le domaine est géré chez <strong>OVH</strong>.
    </p>
    <p>Tout est optimisé à la main — avec beaucoup d'amour et de patience.</p>
    <div class="about-stack">
      <a href="https://gohugo.io/" class="stack-tag" target="_blank" rel="noopener">Hugo</a>
      <a href="https://github.com/adityatelange/hugo-PaperMod" class="stack-tag" target="_blank" rel="noopener">PaperMod</a>
      <a href="https://github.com/" class="stack-tag" target="_blank" rel="noopener">GitHub</a>
      <a href="https://www.netlify.com/" class="stack-tag" target="_blank" rel="noopener">Netlify</a>
      <a href="https://www.ovhcloud.com/" class="stack-tag" target="_blank" rel="noopener">OVH</a>
    </div>
  </section>

  <hr class="about-rule">

  <!-- SECTION : MATÉRIEL -->
  <section class="about-section">
    <span class="about-section__label">03 — Setup</span>
    <h2 class="about-section__title">Mon matériel</h2>
    <p>
      Une page dédiée recense l'ensemble du matériel que j'utilise au quotidien
      — mis à jour au fil de l'évolution de mon setup.
    </p>
    <p>
      Les liens proposés sont des liens affiliés. Cela ne change rien pour vous
      et ça vous permet de me soutenir.
    </p>
    <div class="about-cta-row">
      <a href="/materiel/" class="about-cta about-cta--secondary">
        Voir mon matériel →
      </a>
    </div>
  </section>

  <hr class="about-rule">

  <!-- SECTION : RÉSEAUX -->
  <section class="about-section">
    <span class="about-section__label">04 — Réseaux</span>
    <h2 class="about-section__title">Me suivre</h2>
    <p>
      Vous souhaitez suivre mes aventures sur les réseaux sociaux ?
      Retrouvez tous mes liens depuis ma page personnelle.
    </p>
    <div class="about-cta-row">
      <a href="https://eckodeath.carrd.co" class="about-cta about-cta--primary" target="_blank" rel="noopener">
        eckodeath.carrd.co →
      </a>
    </div>
  </section>

  <!-- FOOTER NOTE COPYRIGHT -->
  <div class="about-footer-note">
    <strong>© eckodeath.fr — Tous droits réservés.</strong><br>
    Les textes, photos et vidéos partagés ici sont le fruit de mon travail et de mes expériences.
    Merci de ne pas les utiliser sans mon autorisation écrite. Si vous souhaitez partager un extrait,
    contactez-moi — je suis toujours ouvert à l'échange.
  </div>

</div>
