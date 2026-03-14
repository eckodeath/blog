---
title: "Projet 12 - 2026 : Avril"
date: 2026-03-12
draft: true
tags: ["photographie", "projet 12", "préambule", "2026", "lifestyle" ]
categories: ["Photographie"]
summary: ""
cover:
    image: ""
    alt: ""
    caption: ""
    relative: false
---


<style>
  :root { --transition: 0.5s ease; }

  [data-theme="light"] {
    --bg:         #ffffff;
    --surface:    #ebe7df;
    --border:     rgba(0,0,0,0.10);
    --text:       #1a1814;
    --text-muted: #6b6459;
    --accent:     #c0392b;
    --tag-bg:     rgba(0,0,0,0.06);
    --overlay:    linear-gradient(to top, rgba(244,241,236,0.92) 0%, transparent 60%);
  }

  [data-theme="dark"] {
    --bg:         #0e0d0b;
    --surface:    #161410;
    --border:     rgba(255,255,255,0.08);
    --text:       #e8e3da;
    --text-muted: #7a7268;
    --accent:     #e05240;
    --tag-bg:     rgba(255,255,255,0.05);
    --overlay:    linear-gradient(to top, rgba(14,13,11,0.95) 0%, transparent 55%);
  }

  @import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;1,300;1,400&family=Space+Mono:wght@400;700&display=swap');

  .pdm-wrap {
    background: var(--bg);
    color: var(--text);
    font-family: 'Cormorant Garamond', Georgia, serif;
    transition: background var(--transition), color var(--transition);
  }

  /* Grain */
  .pdm-wrap::before {
    content: '';
    position: fixed;
    inset: 0;
    background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.85' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.05'/%3E%3C/svg%3E");
    pointer-events: none;
    z-index: 999;
  }

  /* Header */
  .pdm-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 1.4rem 2.5rem;
    border-bottom: 1px solid var(--border);
    transition: border-color var(--transition);
  }

  .pdm-site-name {
    font-family: 'Space Mono', monospace;
    font-size: 0.78rem;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: var(--text-muted);
    text-decoration: none;
  }
  .pdm-site-name span { color: var(--accent); }

  .pdm-header-right { display: flex; align-items: center; gap: 1.8rem; }

  .pdm-back {
    font-family: 'Space Mono', monospace;
    font-size: 0.68rem;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--text-muted);
    text-decoration: none;
    transition: color 0.2s;
  }
  .pdm-back:hover { color: var(--text); }

  .pdm-toggle {
    background: none;
    border: 1px solid var(--border);
    cursor: pointer;
    width: 36px;
    height: 36px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    color: var(--text-muted);
    transition: border-color var(--transition), background 0.2s, color 0.2s;
  }
  .pdm-toggle:hover { background: var(--tag-bg); color: var(--text); }

  [data-theme="light"] .pdm-icon-moon { display: none; }
  [data-theme="dark"]  .pdm-icon-sun  { display: none; }

  /* Section label */
  .pdm-label {
    font-family: 'Space Mono', monospace;
    font-size: 0.65rem;
    letter-spacing: 0.22em;
    text-transform: uppercase;
    color: var(--accent);
    display: flex;
    align-items: center;
    gap: 0.6rem;
    margin-bottom: 0.7rem;
  }
  .pdm-label::after {
    content: '';
    display: block;
    width: 30px;
    height: 1px;
    background: var(--accent);
    opacity: 0.5;
  }

  /* Main */
  .pdm-main {
    max-width: 1080px;
    margin: 0 auto;
    padding: 3.5rem 2.5rem 5rem;
  }

  /* Hero */
  .pdm-hero {
    position: relative;
    width: 100%;
    overflow: hidden;
    border-radius: 2px;
    margin-bottom: 2.2rem;
    opacity: 0;
    animation: pdmFadeUp 0.9s 0.1s ease forwards;
  }
  .pdm-hero img {
    width: 100%;
    height: auto;
    display: block;
    transition: transform 8s ease;
  }
  .pdm-hero:hover img { transform: scale(1.02); }

  .pdm-overlay {
    position: absolute;
    inset: 0;
    background: var(--overlay);
    pointer-events: none;
    transition: background var(--transition);
  }

  .pdm-badge {
    position: absolute;
    top: 1.2rem;
    right: 1.2rem;
    background: var(--bg);
    color: var(--text);
    font-family: 'Space Mono', monospace;
    font-size: 0.62rem;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    padding: 0.35rem 0.75rem;
    border-radius: 1px;
    transition: background var(--transition), color var(--transition);
  }

  .pdm-exif {
    position: absolute;
    bottom: 1.2rem;
    left: 1.2rem;
    display: flex;
    gap: 1.2rem;
    font-family: 'Space Mono', monospace;
    font-size: 0.58rem;
    letter-spacing: 0.1em;
    color: rgba(255,255,255,0.72);
  }
  .pdm-exif-item { display: flex; flex-direction: column; align-items: flex-start; gap: 0.1rem; }
  .pdm-exif-label { opacity: 0.55; font-size: 0.5rem; text-transform: uppercase; letter-spacing: 0.15em; }

  /* Meta row */
  .pdm-meta {
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
    gap: 2rem;
    margin-bottom: 2.4rem;
    opacity: 0;
    animation: pdmFadeUp 0.9s 0.25s ease forwards;
  }

  .pdm-title {
    font-size: clamp(1.9rem, 4vw, 2.8rem);
    font-weight: 300;
    line-height: 1.15;
    letter-spacing: -0.01em;
    margin-bottom: 0.5rem;
  }
  .pdm-title em { font-style: italic; color: var(--text-muted); }

  .pdm-date {
    font-family: 'Space Mono', monospace;
    font-size: 0.65rem;
    color: var(--text-muted);
    letter-spacing: 0.12em;
  }

  .pdm-tags { display: flex; flex-wrap: wrap; justify-content: flex-end; gap: 0.4rem; }
  .pdm-tag {
    font-family: 'Space Mono', monospace;
    font-size: 0.58rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    background: var(--tag-bg);
    color: var(--text-muted);
    padding: 0.25rem 0.6rem;
    border-radius: 1px;
    transition: background var(--transition);
  }

  .pdm-divider {
    width: 100%;
    height: 1px;
    background: var(--border);
    margin-bottom: 2.4rem;
    transition: background var(--transition);
  }

  /* Content grid */
  .pdm-grid {
    display: grid;
    grid-template-columns: 1fr 300px;
    gap: 4rem;
    opacity: 0;
    animation: pdmFadeUp 0.9s 0.4s ease forwards;
  }

  .pdm-body p {
    font-size: 1.2rem;
    line-height: 1.82;
    color: var(--text);
    margin-bottom: 1.4rem;
    font-weight: 300;
  }
  .pdm-body p:first-child::first-letter {
    font-size: 3.5rem;
    float: left;
    line-height: 0.85;
    margin-right: 0.12em;
    font-style: italic;
    color: var(--accent);
  }

  /* Sidebar */
  .pdm-sidebar-block { margin-bottom: 2.4rem; }
  .pdm-sidebar-block .pdm-label { margin-bottom: 1rem; }

  .pdm-gear { list-style: none; }
  .pdm-gear li {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    padding: 0.55rem 0;
    border-bottom: 1px solid var(--border);
    font-size: 0.95rem;
    font-weight: 300;
    transition: border-color var(--transition);
  }
  .pdm-gear li:last-child { border-bottom: none; }
  .pdm-gear-key {
    font-family: 'Space Mono', monospace;
    font-size: 0.6rem;
    text-transform: uppercase;
    letter-spacing: 0.12em;
    color: var(--text-muted);
  }
  .pdm-gear-val { font-style: italic; }

  .pdm-location {
    background: var(--surface);
    padding: 1.1rem 1.3rem;
    border-radius: 2px;
    transition: background var(--transition);
  }
  .pdm-location-name { font-size: 1.05rem; font-weight: 300; margin-bottom: 0.2rem; }
  .pdm-location-detail {
    font-family: 'Space Mono', monospace;
    font-size: 0.6rem;
    color: var(--text-muted);
    letter-spacing: 0.1em;
  }

  /* Nav */
  .pdm-nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 3rem;
    margin-top: 3rem;
    border-top: 1px solid var(--border);
    opacity: 0;
    animation: pdmFadeUp 0.9s 0.55s ease forwards;
    transition: border-color var(--transition);
  }
  .pdm-nav-link { display: flex; flex-direction: column; gap: 0.3rem; text-decoration: none; color: var(--text); }
  .pdm-nav-link.next { align-items: flex-end; }
  .pdm-nav-dir {
    font-family: 'Space Mono', monospace;
    font-size: 0.58rem;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    color: var(--text-muted);
  }
  .pdm-nav-title { font-size: 1rem; font-weight: 300; font-style: italic; transition: color 0.2s; }
  .pdm-nav-link:hover .pdm-nav-title { color: var(--accent); }

  /* Animation */
  @keyframes pdmFadeUp {
    from { opacity: 0; transform: translateY(16px); }
    to   { opacity: 1; transform: translateY(0); }
  }

  /* Footer */
  .pdm-footer {
    text-align: center;
    padding: 2rem;
    border-top: 1px solid var(--border);
    font-family: 'Space Mono', monospace;
    font-size: 0.6rem;
    letter-spacing: 0.14em;
    color: var(--text-muted);
    text-transform: uppercase;
    transition: border-color var(--transition);
  }

  /* Responsive */
  @media (max-width: 720px) {
    .pdm-header { padding: 1.2rem 1.4rem; }
    .pdm-main { padding: 2.4rem 1.4rem 4rem; }
    .pdm-grid { grid-template-columns: 1fr; gap: 2.5rem; }
    .pdm-meta { flex-direction: column; gap: 1rem; }
    .pdm-tags { justify-content: flex-start; }
    .pdm-exif { display: none; }
  }
</style>

  <!-- ── Hero — remplacez src par votre photo ── -->
  <div class="pdm-hero">
      <img src="/posts/2026_projet_12/Janvier/2026-Projet12-Janvier.png" alt="Lumière de crête — Mars 2026" />
      <div class="pdm-overlay"></div>
      <span class="pdm-badge">Mars 2026</span>
      <div class="pdm-exif">
        <div class="pdm-exif-item"><span class="pdm-exif-label">Focale</span><span>35 mm</span></div>
        <div class="pdm-exif-item"><span class="pdm-exif-label">Ouverture</span><span>f/2.8</span></div>
        <div class="pdm-exif-item"><span class="pdm-exif-label">Vitesse</span><span>1/500 s</span></div>
        <div class="pdm-exif-item"><span class="pdm-exif-label">ISO</span><span>200</span></div>
      </div>
    </div>

  <!-- ── Meta ── -->
  <div class="pdm-meta">
      <div>
        <div class="pdm-label">Photo du Mois</div>
        <h1 class="pdm-title">Lumière <em>de crête</em></h1>
        <p class="pdm-date">10 mars 2026 &nbsp;·&nbsp; par Kurt Grava</p>
      </div>
      <div style="display:flex;flex-direction:column;align-items:flex-end;flex-shrink:0">
        <div class="pdm-tags">
          <span class="pdm-tag">Paysage</span>
          <span class="pdm-tag">Montagne</span>
          <span class="pdm-tag">Lumière dorée</span>
          <span class="pdm-tag">Fujifilm</span>
        </div>
      </div>
    </div>

  <div class="pdm-divider"></div>

  <!-- ── Contenu + Sidebar ── -->
  <div class="pdm-grid">

  <article class="pdm-body">
        <p>
          Ce cliché est né d'une patience de plusieurs heures, perché à 2 400 mètres d'altitude,
          dans l'attente de ce moment précis où la lumière rasante vient caresser la crête enneigée.
          Il y a quelque chose d'absolument unique dans cette qualité de lumière de fin de journée
          en montagne — une chaleur presque contradictoire avec le froid mordant de l'air.
        </p>
        <p>
          J'ai choisi une focale de 35 mm pour conserver ce sentiment de présence, d'immersion
          dans la scène. Un grand-angle aurait aplati les volumes, un téléobjectif aurait isolé
          le sujet de son contexte. Ici, on est dedans — le ciel, la roche, la neige et la lumière
          forment un tout cohérent.
        </p>
        <p>
          Le traitement en post-production est volontairement minimaliste : une légère récupération
          dans les hautes lumières, un tout petit push sur les noirs pour préserver la profondeur,
          rien de plus. Je voulais que la photo reste honnête par rapport à ce que j'ai vécu sur place.
        </p>
      </article>

  <aside>
        <div class="pdm-sidebar-block">
          <div class="pdm-label">Matériel</div>
          <ul class="pdm-gear">
            <li><span class="pdm-gear-key">Boîtier</span><span class="pdm-gear-val">Fujifilm X-T5</span></li>
            <li><span class="pdm-gear-key">Objectif</span><span class="pdm-gear-val">XF 35mm f/2 R WR</span></li>
            <li><span class="pdm-gear-key">Trépied</span><span class="pdm-gear-val">Gitzo Traveler</span></li>
            <li><span class="pdm-gear-key">Logiciel</span><span class="pdm-gear-val">Lightroom Classic</span></li>
          </ul>
        </div>
        <div class="pdm-sidebar-block">
          <div class="pdm-label">Lieu</div>
          <div class="pdm-location">
            <p class="pdm-location-name">Massif de Belledonne</p>
            <p class="pdm-location-detail">Isère, France &nbsp;·&nbsp; 45°12′N 5°58′E</p>
          </div>
        </div>
      </aside>

  </div>

</div>

<script>
  const wrap = document.getElementById('pdm-wrap');
  const btn  = document.getElementById('pdmToggle');

  // Démarre toujours en mode clair
  wrap.setAttribute('data-theme', 'light');

  // Bouton de bascule manuel toujours actif
  btn.addEventListener('click', () => {
    const current = wrap.getAttribute('data-theme');
    wrap.setAttribute('data-theme', current === 'dark' ? 'light' : 'dark');
  });
</script>
