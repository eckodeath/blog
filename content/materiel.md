---
title: "Mon matériel"
---

<style>
* { box-sizing: border-box; margin: 0; padding: 0; }

.materiel-wrap {
  max-width: 720px;
  padding: 2rem 0;
}

.materiel-group {
  margin-bottom: 8rem;
}

.materiel-section-label {
  font-size: 16px;
  font-weight: 700;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  color: #999;
  margin-bottom: 2rem;
  display: flex;
  align-items: center;
  gap: 12px;
}

.materiel-section-label::after {
  content: '';
  flex: 1;
  height: 1.5px;
  background: #e5e5e5;
}

.materiel-row {
  display: grid;
  grid-template-columns: 256px 1fr auto;
  align-items: center;
  gap: 16px;
  padding: 0;
  border-bottom: 0.5px solid #e5e5e5;
}

.materiel-row:first-of-type {
  border-top: 0.5px solid #e5e5e5;
}

.materiel-thumb {
  width: 256px;
  height: 256px;
  overflow: hidden;
  flex-shrink: 0;
}

.materiel-thumb img {
  width: 100%;
  height: 100%;
  object-fit: contain;
}

.materiel-name {
  font-size: 15px;
  font-weight: 600;
  line-height: 1.3;
  color: #111 !important;
}

.materiel-desc {
  font-size: 12px;
  color: #aaa;
  margin-top: 3px;
}

.materiel-link {
  font-size: 14px;
  color: #bbb;
  text-decoration: none;
  flex-shrink: 0;
}

@media (prefers-color-scheme: dark) {
  .materiel-section-label { color: #666; }
  .materiel-section-label::after { background: #2a2a2a; }
  .materiel-row { border-bottom-color: #2a2a2a; }
  .materiel-row:first-of-type { border-top-color: #2a2a2a; }
  .materiel-name { color: #f0f0f0; }
  .materiel-desc { color: #555; }
  .materiel-link { color: #444; }
}
</style>

<div class="materiel-wrap">

  <!-- Apple -->
  <div class="materiel-group">
    <div class="materiel-section-label">Apple</div>

  <div class="materiel-row">
      <div class="materiel-thumb"><img src="/images/materiel/iphone_16_pro_max_matos.png" alt="iPhone 16 Pro Max"></div>
      <div><div class="materiel-name">iPhone 16 Pro Max</div><div class="materiel-desc">Smartphone</div></div>
      <a class="materiel-link" href="https://amzn.to/3TRxlOU" target="_blank" rel="noopener">↗</a>
    </div>

  <div class="materiel-row">
      <div class="materiel-thumb"><img src="/images/materiel/MacBook_Air_M4_matos.png" alt="MacBook Air M4"></div>
      <div><div class="materiel-name">MacBook Air M4</div><div class="materiel-desc">Ordinateur portable</div></div>
      <a class="materiel-link" href="https://amzn.to/4fk7itH" target="_blank" rel="noopener">↗</a>
    </div>

  <div class="materiel-row">
      <div class="materiel-thumb"><img src="/images/materiel/ipad_pro_2017_matos.png" alt="iPad Pro 2017"></div>
      <div><div class="materiel-name">iPad Pro 2017</div><div class="materiel-desc">Tablette</div></div>
      <a class="materiel-link" href="https://amzn.to/3GTgqcc" target="_blank" rel="noopener">↗</a>
    </div>

  <div class="materiel-row">
      <div class="materiel-thumb"><img src="/images/materiel/apple_watch_series_7_matos.png" alt="Apple Watch Series 7"></div>
      <div><div class="materiel-name">Apple Watch Series 7</div><div class="materiel-desc">Montre connectée</div></div>
      <a class="materiel-link" href="https://amzn.to/4eNetdT" target="_blank" rel="noopener">↗</a>
    </div>
    
  <div class="materiel-row">
      <div class="materiel-thumb"><img src="/images/materiel/Porte_cartes_magsafe_matos.png" alt="Porte Cartes Magsafe"></div>
      <div><div class="materiel-name">Porte Cartes</div><div class="materiel-desc">Accessoires</div></div>
      <a class="materiel-link" href="https://amzn.to/4thA2sK" target="_blank" rel="noopener">↗</a>
    </div>
  </div>

  <div class="materiel-row">
      <div class="materiel-thumb"><img src="/images/materiel/AirPods_Pro_2_matos.png" alt="AirPods Pro 2"></div>
      <div><div class="materiel-name">AirPods Pro 2</div><div class="materiel-desc">Écouteurs</div></div>
      <a class="materiel-link" href="https://amzn.to/45JWXVk" target="_blank" rel="noopener">↗</a>
    </div>
  </div>

  <!-- Photo & Vidéo -->
  <div class="materiel-group">
    <div class="materiel-section-label">Photo & Vidéo</div>

  <div class="materiel-row">
      <div class="materiel-thumb"><img src="/images/materiel/sony_nex_5r_matos.png" alt="Sony NEX-5R"></div>
      <div><div class="materiel-name">Sony NEX-5R</div><div class="materiel-desc">Appareil photo hybride</div></div>
      <span class="materiel-link">↗</span>
    </div>

  <div class="materiel-row">
      <div class="materiel-thumb"><img src="/images/materiel/sony_16_50_matos.png" alt="Sony 16-50mm"></div>
      <div><div class="materiel-name">Sony 16-50mm F3.5-5.6</div><div class="materiel-desc">Objectif grand angle</div></div>
      <a class="materiel-link" href="https://amzn.to/3ISPdab" target="_blank" rel="noopener">↗</a>
    </div>

  <div class="materiel-row">
      <div class="materiel-thumb"><img src="/images/materiel/sony_55_210_matos.png" alt="Sony 55-210mm"></div>
      <div><div class="materiel-name">Sony 55-210mm F4.5-6.3</div><div class="materiel-desc">Objectif téléphoto</div></div>
      <a class="materiel-link" href="https://amzn.to/4mLRR07" target="_blank" rel="noopener">↗</a>
    </div>

  <div class="materiel-row">
      <div class="materiel-thumb"><img src="/images/materiel/smallrig_ct10_matos.png" alt="Trépied SmallRig CT-10"></div>
      <div><div class="materiel-name">Trépied SmallRig CT-10</div><div class="materiel-desc">Trépied compact</div></div>
      <a class="materiel-link" href="https://amzn.to/3Hk3Vq1" target="_blank" rel="noopener">↗</a>
    </div>
  </div>

  <!-- Accessoires & Stockage -->
  <div class="materiel-group">
    <div class="materiel-section-label">Accessoires & Stockage</div>

  <div class="materiel-row">
      <div class="materiel-thumb"><img src="/images/materiel/Asus_ProArt_matos.png" alt="Asus ProArt"></div>
      <div><div class="materiel-name">Asus ProArt PA27JCV</div><div class="materiel-desc">Moniteur 5K</div></div>
      <a class="materiel-link" href="https://amzn.to/4v0Q5gg" target="_blank" rel="noopener">↗</a>
    </div>

  <div class="materiel-row">
      <div class="materiel-thumb"><img src="/images/materiel/Lexar_ES5_matos.png" alt="Lexar ES5"></div>
      <div><div class="materiel-name">Lexar ES5</div><div class="materiel-desc">SSD externe</div></div>
      <a class="materiel-link" href="https://amzn.to/4lccDoi" target="_blank" rel="noopener">↗</a>
    </div>

  <div class="materiel-row">
      <div class="materiel-thumb"><img src="/images/materiel/ringconn_gen2_matos.png" alt="RingConn Gen 2"></div>
      <div><div class="materiel-name">RingConn Gen 2</div><div class="materiel-desc">Bague connectée</div></div>
      <a class="materiel-link" href="https://amzn.to/4luMrFM" target="_blank" rel="noopener">↗</a>
    </div>

  <div class="materiel-row">
      <div class="materiel-thumb"><img src="/images/materiel/quechua_nh_900_matos.png" alt="Quechua NH900 Explore"></div>
      <div><div class="materiel-name">Quechua NH900 Explore</div><div class="materiel-desc">Sac à dos 30L</div></div>
      <a class="materiel-link" href="https://www.decathlon.fr/p/sac-a-dos-appareil-photo-randonnee-30l-nh-explorer-900-focus/_/R-p-344239" target="_blank" rel="noopener">↗</a>
    </div>
  </div>

</div>
