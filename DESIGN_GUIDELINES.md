# 🎨 GUIDELINES UI/UX - Site Académique Adrien Cloutier

## 📋 TABLE DES MATIÈRES

1. [Audit du design actuel](#audit)
2. [Principes de design académique](#principes)
3. [Typographie](#typographie)
4. [Palette de couleurs](#couleurs)
5. [Composants UI recommandés](#composants)
6. [Hiérarchie visuelle](#hierarchie)
7. [Footer académique](#footer)
8. [Implémentation](#implementation)
9. [Checklist de mise en œuvre](#checklist)

---

## 🔍 AUDIT DU DESIGN ACTUEL {#audit}

### Points positifs ✅
- Template HTML5 UP "Read Only" solide et responsive
- Palette bleue professionnelle (#2563eb)
- Navigation sidebar claire
- Bouton de langue présent
- Structure bilingue cohérente

### Points à améliorer ⚠️
1. **Typographie standard** → Manque de caractère académique
2. **Hero section peu impactante** → Pas assez différenciée
3. **Cards de projets génériques** → Manque de hiérarchie visuelle
4. **Espacement perfectible** → Densité inégale
5. **Footer basique** → Ne met pas en valeur les liens académiques clés
6. **Sections CLESSN/CAPP** → Manquent de structure visuelle distinctive
7. **Icônes trop présentes** → Effet "marketing" plutôt qu'académique

---

## 🎯 PRINCIPES DE DESIGN ACADÉMIQUE {#principes}

### 1. Sobriété et Crédibilité
- **Moins de couleurs**, plus d'espaces blancs
- **Typographie lisible** (serif pour titres, sans-serif pour corps)
- **Hiérarchie claire** (titres → sous-titres → corps)
- **Pas d'effets flashy** (animations discrètes)

### 2. Scannabilité
- **Sections clairement délimitées** (bordures, espacement)
- **Titres explicites** ("Recherche" plutôt que "Mon travail")
- **Cards uniformes** pour projets/centres/conférences
- **Icônes minimalistes** et professionnelles

### 3. Hiérarchie de l'Information
**Ordre d'importance:**
1. Nom + Statut + Champs de recherche (Hero)
2. Thèse + Postdoc + Défense 2026
3. Centres de recherche (CLESSN, CAPP)
4. Projets majeurs (Radar+, RFICS, EIOM)
5. Publications + Conférences
6. Enseignement + Compétences
7. Contact

### 4. Accessibilité Académique
- **Contrastes suffisants** (WCAG AA minimum)
- **Taille de police lisible** (16px minimum)
- **Liens clairement identifiables**
- **Navigation au clavier** fonctionnelle

---

## 📝 TYPOGRAPHIE {#typographie}

### Police recommandée: **Crimson Pro + Inter**

**Pourquoi ce choix?**
- **Crimson Pro** (serif) → Élégance académique pour titres
- **Inter** (sans-serif) → Lisibilité maximale pour corps de texte
- Combinaison utilisée par Harvard, MIT, Stanford

### Hiérarchie typographique

```css
H1: 2.5rem (40px) - Crimson Pro Bold - Nom principal
H2: 2rem (32px) - Crimson Pro Bold - Titres de sections
H3: 1.5rem (24px) - Crimson Pro SemiBold - Sous-sections
H4: 1.25rem (20px) - Crimson Pro SemiBold - Titres de cards
Body: 1rem (16px) - Inter Regular - Corps de texte
Small: 0.9rem (14px) - Inter Regular - Métadonnées
```

### Interlignage (line-height)
- **Titres:** 1.3 (serré pour élégance)
- **Corps:** 1.7 (aéré pour lisibilité)

### Espacement vertical
- Entre sections: 4rem (64px)
- Entre paragraphes: 1.25rem (20px)
- Entre titre et contenu: 2rem (32px)

---

## 🎨 PALETTE DE COULEURS {#couleurs}

### Bleu Académique (couleur principale)

```
Bleu Principal: #2563eb (Bleu professionnel)
Bleu Foncé: #1e40af (Header, liens hover)
Bleu Très Foncé: #1e3a8a (Gradients)
Bleu Clair: #3b82f6 (Accents)
Bleu Très Clair: #eff6ff (Backgrounds)
```

### Gris Académique (textes et backgrounds)

```
Gris Très Foncé: #111827 (Titres principaux)
Gris Foncé: #1f2937 (Titres secondaires)
Gris Moyen Foncé: #374151 (Corps de texte)
Gris Moyen: #4b5563 (Texte secondaire)
Gris Moyen Clair: #6b7280 (Métadonnées)
Gris Clair: #9ca3af (Icônes)
Gris Très Clair: #e5e7eb (Bordures)
Background: #f9fafb (Footer)
Blanc: #ffffff (Cards, contenus)
```

### Règles d'usage

1. **Header:** Gradient bleu (#1e3a8a → #2563eb)
2. **Titres H1-H2:** Gris très foncé (#111827)
3. **Titres H3-H4:** Bleu foncé (#1e40af)
4. **Corps de texte:** Gris moyen foncé (#374151)
5. **Liens:** Bleu principal (#2563eb)
6. **Bordures:** Gris très clair (#e5e7eb)
7. **Backgrounds cards:** Blanc (#ffffff)
8. **Footer:** Gris très clair (#f9fafb)

---

## 🧩 COMPOSANTS UI RECOMMANDÉS {#composants}

### 1. Cards Académiques (`.academic-card`)

**Usage:** Projets généraux, éléments de liste structurés

**Caractéristiques:**
- Background blanc
- Bordure grise (#e5e7eb)
- Border-radius: 0.5rem (8px)
- Padding: 2rem (32px)
- Shadow subtile au repos
- Shadow accentuée + translateY au hover
- Bordure bleue au hover

**Exemple HTML:**
```html
<div class="academic-card">
  <h4><a href="[url]">Titre du projet</a></h4>
  <span class="card-meta">Institution ou contexte</span>
  <p>Description du projet...</p>
</div>
```

### 2. Cards Centres de Recherche (`.research-center-card`)

**Usage:** CLESSN, CAPP

**Caractéristiques:**
- Background gradient subtil (blanc → gris clair)
- Bordure 2px (#e5e7eb)
- Barre verticale bleue à gauche (4px)
- Padding: 2rem
- Pas de hover agressif (sobriété)

**Exemple HTML:**
```html
<div class="research-center-card">
  <h4><a href="[url]" target="_blank">CLESSN</a></h4>
  <span class="center-subtitle">Chaire de leadership...</span>
  <p>Description complète...</p>
  <ul class="actions">
    <li><a href="[url]" class="button small">Visiter le site</a></li>
  </ul>
</div>
```

### 3. Cards Projets (`.project-card`)

**Usage:** Datagotchi, Quorum, projets visuels

**Caractéristiques:**
- Image colorée en haut (gradient personnalisé)
- Contenu en bas (padding 2rem)
- Hover: translateY(-4px) + shadow importante
- Transition fluide (0.3s ease)

**Exemple HTML:**
```html
<div class="project-card">
  <a href="[url]" target="_blank" class="image">
    <div class="project-image" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);">
      Nom du Projet
    </div>
  </a>
  <div class="project-content">
    <h4><a href="[url]">Titre</a></h4>
    <p>Description...</p>
  </div>
</div>
```

### 4. Cards Conférences (`.conference-card`)

**Usage:** Talks, présentations

**Caractéristiques:**
- Image stylisée en haut (180px height)
- Métadonnées (institution, date)
- Contenu détaillé
- Hover élégant

**Exemple HTML:**
```html
<div class="conference-card">
  <a href="[url]" target="_blank" class="image">
    <div class="conference-image" style="background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);">
      Sujet abrégé
    </div>
  </a>
  <div class="conference-content">
    <h4><a href="[url]">Titre complet</a></h4>
    <span class="conference-meta">Institution</span>
    <p>Description...</p>
  </div>
</div>
```

### 5. Grid Layout Responsive

**Deux colonnes:**
```html
<div class="row academic-cards">
  <div class="academic-card">...</div>
  <div class="academic-card">...</div>
</div>
```

**Projets en grid:**
```html
<div class="projects-grid">
  <div class="project-card">...</div>
  <div class="project-card">...</div>
</div>
```

---

## 📊 HIÉRARCHIE VISUELLE {#hierarchie}

### Section "À propos" (#one)

**Structure recommandée:**

```
[Image cover - graffiti]

H2: Adrien Cloutier
P: PhD Candidate | Université Laval | Defense Fall 2026
<div class="accent-line"></div>

<p class="section-intro">
  Paragraphe introductif résumant la thèse...
</p>

[4 paragraphes détaillés]
- Thèse + FRQ + Spécialisations
- EIOM + RFICS
- Radar+
- Enseignement + Postdoc
```

### Section "Mon travail" (#two)

**Structure recommandée:**

```
H3: Projets et réalisations

<p class="section-intro">
  Texte introductif...
</p>

<ul class="feature-icons">
  [6 items avec icônes]
</ul>
```

### Section "CLESSN / CAPP" (#three)

**Structure recommandée:**

```
H3: CLESSN / CAPP

<p class="section-intro">
  Rôle de co-coordonnateur...
</p>

<div class="row academic-cards">
  <div class="research-center-card">[CLESSN]</div>
  <div class="research-center-card">[CAPP]</div>
</div>

H4: Projets liés

<div class="projects-grid">
  <div class="project-card">[Datagotchi]</div>
  <div class="project-card">[Quorum]</div>
</div>
```

### Section "Conférences" (#four)

**Structure recommandée:**

```
H3: Conférences

<p class="section-intro">
  Description des conférences...
</p>

<div class="conference-card">
  [Méthode agile]
</div>

[Structure extensible pour futures conférences]
```

---

## 🦶 FOOTER ACADÉMIQUE {#footer}

### Structure complète recommandée

```html
<section id="footer">
  <div class="academic-footer">
    <div class="footer-links">

      <!-- Colonne 1: Recherche -->
      <div class="footer-column">
        <h4>Recherche</h4>
        <ul>
          <li><a href="https://scholar.google.com/citations?user=RXAdvoMAAAAJ">
            <i class="fas fa-graduation-cap"></i> Google Scholar
          </a></li>
          <li><a href="https://www.clessn.com/radar/index.html">
            <i class="fas fa-broadcast-tower"></i> Radar+
          </a></li>
          <li><a href="https://www.clessn.com/">
            <i class="fas fa-university"></i> CLESSN
          </a></li>
          <li><a href="https://capp-ulaval.ca/">
            <i class="fas fa-chart-line"></i> CAPP
          </a></li>
        </ul>
      </div>

      <!-- Colonne 2: Enseignement & Réseaux -->
      <div class="footer-column">
        <h4>Enseignement & Réseaux</h4>
        <ul>
          <li><a href="https://eiom.ca">
            <i class="fas fa-chalkboard-teacher"></i> EIOM
          </a></li>
          <li><a href="https://rfics.org">
            <i class="fas fa-globe"></i> RFICS
          </a></li>
          <li><a href="https://www.notion.com/@adri01">
            <i class="fas fa-book"></i> Templates Notion
          </a></li>
        </ul>
      </div>

      <!-- Colonne 3: Projets & Contact -->
      <div class="footer-column">
        <h4>Projets & Contact</h4>
        <ul>
          <li><a href="https://www.datagotchi.com/">
            <i class="fas fa-gamepad"></i> Datagotchi
          </a></li>
          <li><a href="https://www.projetquorum.com/">
            <i class="fas fa-comments"></i> Projet Quorum
          </a></li>
          <li><a href="mailto:ADCLO2@ulaval.ca">
            <i class="fas fa-envelope"></i> ADCLO2@ulaval.ca
          </a></li>
        </ul>
      </div>

    </div>
  </div>

  <div class="container">
    <ul class="copyright">
      <li>&copy; 2024-2026 Adrien Cloutier. All rights reserved.</li>
      <li>Design: <a href="http://html5up.net">HTML5 UP</a></li>
    </ul>
  </div>
</section>
```

---

## 🚀 IMPLÉMENTATION {#implementation}

### Étape 1: Intégrer le nouveau CSS

**Modifier le `<head>` de index.html et index_en.html:**

```html
<head>
  <title>Adrien Cloutier - Doctorant en science politique</title>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no" />

  <!-- CSS de base -->
  <link rel="stylesheet" href="assets/css/main.css" />
  <link rel="stylesheet" href="assets/css/custom.css" />

  <!-- NOUVEAU: CSS académique amélioré -->
  <link rel="stylesheet" href="assets/css/academic-enhanced.css" />

  <!-- Google Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <!-- Meta tags SEO/bilinguisme -->
  <link rel="alternate" hreflang="en" href="https://adriencloutier.com/index_en.html" />
  <link rel="alternate" hreflang="fr" href="https://adriencloutier.com/" />
  <link rel="canonical" href="https://adriencloutier.com/" />
</head>
```

### Étape 2: Appliquer les classes CSS aux composants existants

**Exemple: Transformer les divs CLESSN/CAPP**

**AVANT:**
```html
<div class="box alt">
  <h4><a href="https://www.clessn.com/">CLESSN</a></h4>
  <p>Description...</p>
</div>
```

**APRÈS:**
```html
<div class="research-center-card">
  <h4><a href="https://www.clessn.com/" target="_blank">CLESSN</a></h4>
  <span class="center-subtitle">Chaire de leadership en enseignement des sciences sociales numériques</span>
  <p>Description...</p>
  <ul class="actions">
    <li><a href="https://www.clessn.com/" target="_blank" class="button small">Visiter le site</a></li>
  </ul>
</div>
```

**Transformer le layout en grid:**

**AVANT:**
```html
<div class="row">
  <div class="col-6 col-12-medium">
    [CLESSN]
  </div>
  <div class="col-6 col-12-medium">
    [CAPP]
  </div>
</div>
```

**APRÈS:**
```html
<div class="row academic-cards">
  <div class="research-center-card">
    [CLESSN]
  </div>
  <div class="research-center-card">
    [CAPP]
  </div>
</div>
```

### Étape 3: Transformer les projets (Datagotchi, Quorum)

**AVANT:**
```html
<div class="features">
  <article>
    <a href="..." class="image">
      <div style="background: gradient...">Datagotchi</div>
    </a>
    <div class="inner">
      <h4>Datagotchi</h4>
      <p>Description...</p>
    </div>
  </article>
</div>
```

**APRÈS:**
```html
<div class="projects-grid">
  <div class="project-card">
    <a href="https://www.datagotchi.com/" target="_blank">
      <div class="project-image" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);">
        Datagotchi
      </div>
    </a>
    <div class="project-content">
      <h4><a href="https://www.datagotchi.com/" target="_blank">Datagotchi</a></h4>
      <p>Description...</p>
    </div>
  </div>

  <div class="project-card">
    [Quorum]
  </div>
</div>
```

### Étape 4: Transformer les conférences

**AVANT:**
```html
<div class="features">
  <article>
    <a href="..." class="image">
      <div style="background: gradient...">Méthode agile</div>
    </a>
    <div class="inner">
      <h4>Titre</h4>
      <p>Description...</p>
    </div>
  </article>
</div>
```

**APRÈS:**
```html
<div class="conference-card">
  <a href="[url]" target="_blank">
    <div class="conference-image" style="background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);">
      Méthode agile<br>en académie
    </div>
  </a>
  <div class="conference-content">
    <h4><a href="[url]" target="_blank">Utilisation de la méthode agile en milieu académique</a></h4>
    <span class="conference-meta">Faculté des sciences sociales, Université Laval</span>
    <p>Description complète...</p>
  </div>
</div>
```

### Étape 5: Ajouter des intros de section

**Ajouter après chaque H3:**

```html
<h3>CLESSN / CAPP</h3>
<p class="section-intro">
  Adrien Cloutier est co-coordonnateur de deux centres de recherche à l'Université Laval...
</p>
```

### Étape 6: Ajouter le footer académique complet

Remplacer le footer actuel par la structure complète décrite dans la section [Footer Académique](#footer).

---

## ✅ CHECKLIST DE MISE EN ŒUVRE {#checklist}

### Phase 1: Intégration CSS
- [ ] Ajouter `academic-enhanced.css` dans le `<head>`
- [ ] Tester le chargement des Google Fonts (Crimson Pro + Inter)
- [ ] Vérifier que les styles s'appliquent correctement

### Phase 2: Composants UI
- [ ] Transformer les cards CLESSN/CAPP (`.research-center-card`)
- [ ] Transformer les projets Datagotchi/Quorum (`.project-card`)
- [ ] Transformer la conférence agile (`.conference-card`)
- [ ] Ajouter les `.section-intro` après chaque H3

### Phase 3: Grid Layouts
- [ ] Remplacer `.row .col-6` par `.row.academic-cards`
- [ ] Remplacer `.features` par `.projects-grid` pour projets
- [ ] Vérifier le responsive (mobile, tablette, desktop)

### Phase 4: Footer Académique
- [ ] Créer les 3 colonnes de footer (`.footer-links`)
- [ ] Ajouter tous les liens: Google Scholar, Radar+, CLESSN, CAPP, EIOM, RFICS, Notion, Datagotchi, Quorum, Contact
- [ ] Ajouter les icônes FontAwesome
- [ ] Tester tous les liens

### Phase 5: Tests
- [ ] Tester la version française (index.html)
- [ ] Tester la version anglaise (index_en.html)
- [ ] Vérifier la navigation au clavier
- [ ] Tester le responsive (320px, 768px, 1024px, 1440px)
- [ ] Vérifier les contrastes (WCAG AA)
- [ ] Tester les hovers sur tous les éléments interactifs

### Phase 6: Optimisations finales
- [ ] Valider le HTML (W3C Validator)
- [ ] Optimiser les images si nécessaire
- [ ] Tester la vitesse de chargement
- [ ] Vérifier le SEO (meta descriptions, alt texts)
- [ ] Tester sur Safari, Chrome, Firefox, Edge

---

## 📐 BREAKPOINTS RESPONSIVE

```css
/* Large Desktop */
@media screen and (min-width: 1681px) {
  /* Max-width: 1200px pour le contenu */
}

/* Desktop */
@media screen and (max-width: 1680px) and (min-width: 1281px) {
  /* Sidebar fixe + contenu fluide */
}

/* Laptop */
@media screen and (max-width: 1280px) and (min-width: 981px) {
  /* Sidebar devient header horizontal */
}

/* Tablet */
@media screen and (max-width: 980px) and (min-width: 737px) {
  /* Grids 2 colonnes → 1 colonne */
  /* Font-size réduite */
}

/* Mobile Large */
@media screen and (max-width: 736px) and (min-width: 481px) {
  /* Tout en 1 colonne */
  /* Padding réduit */
}

/* Mobile Small */
@media screen and (max-width: 480px) {
  /* Optimisation extrême */
  /* Font-size minimum */
}
```

---

## 🎯 RÉSULTAT ATTENDU

### Avant → Après

**AVANT:**
- Site générique avec template de base
- Typographie standard
- Cards peu différenciées
- Footer minimaliste
- Hiérarchie visuelle faible

**APRÈS:**
- **Site académique professionnel de haut niveau**
- **Typographie élégante** (Crimson Pro + Inter)
- **Cards structurées et cohérentes** (recherche, projets, conférences)
- **Footer académique complet** (tous les liens importants)
- **Hiérarchie visuelle claire** (scannabilité maximale)
- **Rendu sobre et crédible** (pas d'effets marketing)
- **Bilinguisme parfait** (FR/EN structurellement identiques)

---

## 📚 RÉFÉRENCES INSPIRANTES

Sites académiques de référence:
- MIT CSAIL: https://www.csail.mit.edu/
- Stanford HCI: https://hci.stanford.edu/
- Harvard Political Science: https://gov.harvard.edu/
- Oxford Digital Humanities: https://www.digital.humanities.ox.ac.uk/

Caractéristiques communes:
- Typographie serif/sans-serif combinée
- Espaces blancs généreux
- Cards uniformes pour projets
- Footer structuré avec liens académiques
- Navigation claire et sobre
- Pas d'animations flashy

---

**Document créé le:** 2026-01-07
**Version:** 1.0
**Auteur:** Claude Sonnet 4.5 (Designer UI/UX)
**Pour:** Adrien Cloutier - adriencloutier.com
