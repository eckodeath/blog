---
title: "Les étapes de migration vers un blog auto-hébergé"
date: 2025-08-02
draft: true
tags: ["Blog", "Hugo", "Netlify", "GitHub", "Indépendance"]
categories: ["Tutoriel"]
summary: ""
cover:
    image: ""
    alt: ""
    caption: ""
    relative: false
---

### Pourquoi j'ai quitté Medium ?

Après plusieurs années à publier mes articles de voyage et autres sur Medium, j'ai commencé à ressentir les limites de la plateforme :

* Peu de contrôle sur la mise en page
* SEO limité et URL peu personnalisables
* Fonctionnalités verrouillées derrière un paywall
* Difficulté à intégrer des composants modernes (carrousels, galeries, scripts, etc.)

En 2025, j'ai pris la décision de migrer vers un blog **auto-hébergé** basé sur **Hugo**, **Netlify**, et **GitHub**. Mon objectif est simple : retrouver la maîtrise totale de mes contenus, du design et du déploiement.

J'en ai parlé plus en détail dans l'article : <a href="https://eckodeath.netlify.app/posts/eckodeath_est_de_retour/" target="_blank">Eckodeath est de retour avec son propre nom de domaine</a>. N'hésitez pas à aller le lire.

---

### Outils utilisés

En faisant mes recherches de liberté sur la toile, je suis tombé sur plusieurs vidéos Youtube et mon choix s'est porté sur ces outils : 

* **Hugo** : générateur de site statique, ultra-rapide
* **Thème PaperMod** : propre, moderne, personnalisable
* **Netlify** : hébergement gratuit avec déploiement Git
* **GitHub** : stockage du code source
* **Visual Studio Code** : édition des fichiers Markdown
* **Terminal + Git** : gestion de version et déploiement

---

### Étapes de la migration

#### 1. Installation de Hugo

Sur **macOS**, j'ai utilisé [Homebrew](https://brew.sh/), le gestionnaire de paquets. Si Homebrew n'est pas installé, commencez par :

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Ensuite, installez Hugo Extended (nécessaire pour certains thèmes comme PaperMod) :

```bash
brew install hugo
```

Vérifiez que l'installation a fonctionné :

```bash
hugo version
```

#### 2. Création du projet Hugo

```bash
hugo new site mon-blog
cd mon-blog
git init
```

#### 3. Intégration du thème PaperMod

```bash
git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
echo 'theme = "PaperMod"' >> hugo.toml
```

#### 4. Configuration du site (`hugo.toml` ou `config.yml`)

Activation de l'image de couverture, du logo, des options PaperMod :

```yaml
params:
  ShowReadingTime: true
  ShowBreadCrumbs: true
  ShowImageInList: true
  ShowImageInSingle: true
  logo: "images/logo-kurt.png"
  ShowBrandLogo: true
```

#### 5. Import des anciens articles

* Export de mes données Medium (fichiers `.html`)
* Reformatage manuel en Markdown dans `content/posts/`
* Ajout de `images = ["photo.jpg"]` dans le front matter

#### 6. Ajout de contenu image + carrousel

* Dossier `content/article-name/index.md` avec images dans le même dossier
* Partials personnalisés dans `layouts/partials/carousel.html` avec Splide.js

#### 7. Déploiement sur Netlify

* Création d'un repo GitHub : `git remote add origin ...`
* Push initial :

```bash
git add .
git commit -m "Initial commit"
git push -u origin main
```

* Connexion du repo à Netlify
* Ajout du fichier `netlify.toml` :

```toml
[build]
  publish = "public"
  command = "hugo"

[context.production.environment]
  HUGO_VERSION = "0.111.3"
```

---

### Résultat

* Mon blog est déployé automatiquement à chaque `git push`
* Les performances sont excellentes (temps de chargement quasi instantané)
* J'ai le contrôle total sur le code, le design, le SEO
* Et surtout : plus aucune dépendance à une plateforme commerciale

---

### Conclusion

Passer à un blog auto-hébergé avec Hugo demande un peu de mise en place, mais le gain en liberté, performance et personnalisation est incomparable.

Je recommande vivement cette solution à tout blogueur technique ou indépendant qui veut reprendre la main sur ses contenus.

<p style="text-align: right;"> A bientôt sur <a href="https://eckodeath.netlify.app">eckodeath.fr</a>
