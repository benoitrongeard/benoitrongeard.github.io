# Instructions GitHub Copilot - CV Benoît Rongeard

## 📋 Vue d'ensemble du projet

Ce projet est une **GitHub Page** servant de **CV en ligne moderne** pour Benoît Rongeard - Tech Lead & Full Stack Developer.

- **URL principale** : https://benoit-rongeard.fr
- **Technologie** : Jekyll (GitHub Pages)
- **Thème de base** : Architect (personnalisé)

## 🎨 Directives de Design

### Charte Graphique

Le design doit être **moderne** et respecter **strictement** les variables de couleurs définies dans `assets/css/style.scss` :

```scss
--primary-color: #667eea;
--secondary-color: #764ba2;
--accent-color: #2879d0;
--text-dark: #2c3e50;
--text-light: #7f8c8d;
--bg-light: #f8f9fa;
--bg-white: #ffffff;
--shadow-color: rgba(0, 0, 0, 0.1);
```

### Style Visuel

- Utiliser des **dégradés** (gradients) pour les éléments visuels importants
- Appliquer des effets **glassmorphism** pour les cartes et sections
- Animations **fluides** et **subtiles** avec `@keyframes`
- Ombres **douces** et **réalistes** (box-shadow)
- Typographie **claire** et **hiérarchisée**

## 💻 Directives CSS/SCSS

Le code CSS doit être :

### 1. Maintenable

- Structure **logique** et **organisée**
- Commentaires pour les sections importantes
- Nommage **cohérent** des classes (BEM recommandé)
- Séparation claire des responsabilités

### 2. Minimaliste

- Éviter les **redondances**
- Pas de code mort ou inutilisé
- Regrouper les propriétés similaires
- Utiliser des **raccourcis** CSS quand approprié

### 3. Optimisé pour SCSS

- **Variables** pour toutes les valeurs réutilisables
- **Mixins** pour les patterns répétitifs
- **Nesting** pour la lisibilité (max 3 niveaux)
- **Fonctions** SCSS si nécessaire
- Import modulaire si le projet grandit

### 4. Performant

- Animations sur `transform` et `opacity` (GPU-accelerated)
- `will-change` pour les animations complexes
- Éviter les sélecteurs trop lourds
- Optimiser les media queries

**Exemple de structure SCSS attendue :**

```scss
// Variables
$breakpoint-mobile: 480px;
$breakpoint-tablet: 768px;

// Mixins
@mixin card-style {
  background: var(--bg-white);
  border-radius: 12px;
  box-shadow: 0 4px 6px var(--shadow-color);
}

// Composants
.component {
  @include card-style;

  &__element {
    // Styles
  }

  @media (max-width: $breakpoint-tablet) {
    // Responsive
  }
}
```

## 🔍 Directives SEO

### Meta Tags (dans `_layouts/default.html`)

- `<title>` descriptif et unique
- `<meta name="description">` pertinente (150-160 caractères)
- `<meta name="keywords">` ciblés
- Open Graph tags pour les réseaux sociaux
- Twitter Card tags
- Favicon et Apple Touch Icon

### Structure HTML

- Utiliser les balises **sémantiques** HTML5 (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`)
- Hiérarchie des titres **logique** (un seul `<h1>`, puis `<h2>`, `<h3>`, etc.)
- Attributs `alt` pour toutes les images
- Liens avec textes **descriptifs**

### Performance

- Images optimisées (format moderne, compression)
- CSS minifié en production
- Chargement asynchrone si nécessaire
- Pas de ressources bloquantes

### Accessibilité

- Contraste de couleurs suffisant (WCAG AA minimum)
- Navigation au clavier fonctionnelle
- Attributs ARIA si nécessaire
- Attributs `lang` appropriés

## 📱 Directives Responsive

Le site doit être **100% responsive** avec une approche **mobile-first**.

### Breakpoints Obligatoires

```scss
// Mobile First
.element {
  // Styles mobile par défaut
}

// Small Mobile
@media (max-width: 480px) {
  // Ajustements petits écrans
}

// Tablet
@media (min-width: 768px) {
  // Styles tablette
}

// Desktop
@media (min-width: 992px) {
  // Styles desktop
}

// Large Desktop
@media (min-width: 1200px) {
  // Ajustements grands écrans
}
```

### Principes Responsive

- **Flexbox** et **Grid** pour les layouts
- Unités **relatives** (`rem`, `em`, `%`, `vw`, `vh`)
- Images **fluides** (`max-width: 100%`)
- Textes **lisibles** sur tous les écrans
- Touch targets **suffisamment grands** sur mobile (min 44x44px)
- Pas de scroll horizontal
- Menu **hamburger** sur mobile si nécessaire

## 📂 Structure du Projet

```
benoitrongeard.github.io/
├── _config.yml           # Configuration Jekyll
├── _layouts/
│   └── default.html      # Template principal
├── assets/
│   └── css/
│       └── style.scss    # Styles SCSS
├── index.md              # Contenu principal (HTML dans Markdown)
├── Gemfile               # Dépendances Ruby
├── Rakefile              # Commandes utiles (rake serve, rake build)
├── CNAME                 # Domaine personnalisé
└── README.md             # Documentation
```

## ⚡ Commandes Utiles

```bash
# Serveur local avec live-reload
rake serve
# ou
bundle exec jekyll serve --livereload

# Build production
rake build
# ou
bundle exec jekyll build

# Installation des dépendances
bundle install
```

## 🎯 Workflow de Développement

1. **Toujours tester en local** avant de commit (`rake serve`)
2. **Vérifier le responsive** sur plusieurs tailles d'écran
3. **Valider le HTML** (W3C Validator)
4. **Tester la performance** (Lighthouse)
5. **Vérifier l'accessibilité** (contraste, navigation clavier)
6. **Optimiser les assets** avant déploiement

## 🚫 À Éviter

- ❌ Ne pas modifier les couleurs sans mettre à jour les variables
- ❌ Ne pas ajouter de bibliothèques CSS externes lourdes (Bootstrap, etc.)
- ❌ Ne pas utiliser `!important` sauf cas exceptionnel
- ❌ Ne pas créer de styles inline dans le HTML
- ❌ Ne pas ignorer les warnings Jekyll lors du build
- ❌ Ne pas casser le responsive existant
- ❌ Ne pas dégrader les performances (garder un score Lighthouse > 90)

## ✅ Best Practices

- ✅ Utiliser les variables CSS pour toutes les valeurs réutilisables
- ✅ Commenter les sections complexes
- ✅ Tester sur Chrome, Firefox, Safari, et mobile
- ✅ Vérifier le rendu avec et sans JavaScript
- ✅ Optimiser les images avant de les ajouter
- ✅ Utiliser des animations subtiles et professionnelles
- ✅ Maintenir une hiérarchie visuelle claire
- ✅ Penser accessibilité dès la conception

## 🎨 Exemples de Patterns à Suivre

### Card Component

```scss
.card {
  background: var(--bg-white);
  border-radius: 12px;
  padding: 2rem;
  box-shadow: 0 4px 6px var(--shadow-color);
  transition: transform 0.3s ease, box-shadow 0.3s ease;

  &:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 12px var(--shadow-color);
  }
}
```

### Gradient Background

```scss
.hero {
  background: linear-gradient(
    135deg,
    var(--primary-color),
    var(--secondary-color)
  );
}
```

### Glassmorphism Effect

```scss
.glass {
  background: rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.2);
}
```

## 📝 Notes Importantes

- Ce site est le **CV professionnel** de Benoît Rongeard
- Chaque changement doit améliorer l'**expérience utilisateur**
- La **simplicité** et la **clarté** priment sur la complexité
- Le design doit rester **professionnel** et **moderne**
- L'objectif est de **mettre en valeur** les compétences et l'expérience

---

**Version** : 1.0  
**Dernière mise à jour** : 2 novembre 2025
