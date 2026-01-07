# 🔄 REFONTE COMPLÈTE - PLAN D'ARCHITECTURE

**Date:** 2026-01-07
**Objectif:** Restructuration complète du site adriencloutier.com avec menu simplifié (12 sections), hiérarchie visuelle forte, et design académique épuré.

---

## 📋 NOUVELLE ARBORESCENCE (12 SECTIONS)

```
adriencloutier.com
├── 1. Accueil / Home (NOUVEAU - ultra-épuré)
├── 2. À propos / About (restructuré)
├── 3. Radar+ (PAGE DÉDIÉE - centrale)
├── 4. EIOM (PAGE DÉDIÉE - essentielle)
├── 5. Publications (simplifié avec catégories)
├── 6. Enseignement et conférences / Teaching & Talks
├── 7. CAPP / CLESSN (synthèse)
├── 8. RFICS (page dédiée)
├── 9. Agilité / Notion (FUSION outils)
├── 10. Galerie / Gallery
├── 11. CV (simplifié)
└── 12. Contact (simplifié)
```

---

## 🔀 MAPPING: ANCIEN → NOUVEAU

### Contenu à déplacer/réorganiser:

| Contenu actuel | Section actuelle | → Nouvelle destination |
|----------------|------------------|------------------------|
| Bio générale | #1 À propos | → #2 À propos (restructuré) |
| Radar+ détaillé | #2 Recherche | → #3 Radar+ (PAGE DÉDIÉE) |
| Postdoc Fox vs CNN | #2 Recherche | → #2 À propos (intégré) |
| EIOM | #5 EIOM (dédiée) | → #4 EIOM (PAGE DÉDIÉE - conservée) |
| Publications | #3 Publications | → #5 Publications (avec catégories) |
| Cours POL-6078 + Méthodologie | #4 Enseignement | → #6 Enseignement et conférences |
| Conférences (agile FSS) | Dispersé | → #6 Enseignement et conférences |
| RFICS | #6 RFICS | → #8 RFICS (ton plus factuel) |
| CLESSN / CAPP | #7 CLESSN/CAPP | → #7 CAPP / CLESSN (renommé, ordre inversé) |
| Projets liés (Datagotchi, Quorum) | #7 CLESSN/CAPP | → #7 CAPP / CLESSN (conservé) |
| Mandats Mitacs | #8 Mandats (dédiée) | → #7 CAPP / CLESSN (projets liés) |
| Scrum Master | #9 Outils & Méthodes | → #9 Agilité / Notion |
| Templates Notion | #9 Outils & Méthodes | → #9 Agilité / Notion |
| Galerie 4 catégories | #10 Galerie | → #10 Galerie (conservé) |
| Téléchargements (CVs, PDFs) | #11 Téléchargements | → #11 CV (boutons directs) |
| Plans de cours PDFs | #11 Téléchargements | → #6 Enseignement (liens dans cours) |
| Rapports Mitacs PDFs | #11 Téléchargements | → #7 CAPP/CLESSN (dans Mitacs) |
| Contact | #12 Contact | → #12 Contact (simplifié) |

### ✅ Garantie: AUCUN contenu perdu

Tout le contenu existant est **réorganisé et hiérarchisé**, pas supprimé:
- **EIOM** → conservée comme PAGE DÉDIÉE (section #4 - essentielle)
- Mandats Mitacs → intégrés dans CAPP/CLESSN (projets appliqués)
- Postdoc → intégré dans À propos
- Téléchargements → boutons directs dans sections respectives
- Scrum + Notion → fusionnés dans Agilité/Notion

---

## 📐 WIREFRAMES SECTION PAR SECTION

### 1️⃣ ACCUEIL / HOME (NOUVEAU - ULTRA-ÉPURÉ)

**Structure:**
```
┌─────────────────────────────────────┐
│         [Photo portrait]            │
│                                     │
│         Adrien Cloutier             │
│ Doctorant en science politique      │
│        Université Laval              │
│                                     │
│ Saillance médiatique • Communication │
│   politique • Méthodes computationnelles│
│                                     │
│ [3-4 lignes max de présentation]   │
│                                     │
│   [Radar+] [Publications] [CV] [Contact]│
└─────────────────────────────────────┘
```

**Contenu FR:**
- **Titre:** Adrien Cloutier
- **Sous-titre:** Doctorant en science politique, Université Laval | Défense 2026
- **Champs:** Saillance médiatique • Communication politique • Méthodes computationnelles
- **Paragraphe (3-4 lignes):**
  > "Je développe Radar+, une infrastructure computationnelle qui mesure la saillance des objets publics dans les médias québécois, canadiens et américains. Ma thèse analyse l'agenda médiatique à l'ère numérique. En 2027, je poursuivrai au postdoctorat à UCLA pour étudier la polarisation médiatique aux États-Unis."

**Contenu EN:**
- **Title:** Adrien Cloutier
- **Subtitle:** PhD Candidate in Political Science, Université Laval | Defense 2026
- **Fields:** Media salience • Political communication • Computational methods
- **Paragraph (3-4 lines):**
  > "I develop Radar+, a computational infrastructure that measures public issue salience in Quebec, Canadian, and American media. My dissertation analyzes the media agenda in the digital age. In 2027, I will pursue a postdoctoral fellowship at UCLA to study media polarization in the United States."

**Boutons:**
- Radar+ → #three
- Publications → #four
- CV → #ten
- Contact → #eleven

**Design:**
- Hero centré, beaucoup d'espace blanc
- Photo portrait circulaire (si disponible)
- Typographie grande et claire
- Boutons bien espacés, call-to-action évidents
- AUCUN texte long, AUCUNE liste

---

### 2️⃣ À PROPOS / ABOUT (RESTRUCTURÉ)

**Structure:**
```
┌─────────────────────────────────────┐
│           À propos                  │
│                                     │
│ [Paragraphe 1: Bio académique]     │
│                                     │
│ [Paragraphe 2: Thèse]               │
│                                     │
│ [Paragraphe 3: Postdoc + méthodologie]│
│                                     │
│ [Liens professionnels]              │
│ • Google Scholar                    │
│ • GitHub                            │
│ • LinkedIn                          │
└─────────────────────────────────────┘
```

**Contenu FR (2-3 paragraphes max):**

**§1 - Bio académique:**
> Adrien Cloutier est doctorant en science politique à l'Université Laval (défense prévue automne 2026), où il consacre ses recherches à la communication politique, à l'agenda médiatique et aux méthodes computationnelles. Il est chargé de cours depuis 2024 et enseigne les outils numériques et la méthodologie quantitative en sciences sociales.

**§2 - Thèse:**
> Sa thèse, intitulée *"Breaking News: Radar+ for Measuring Media Salience in the Digital Age"*, développe une infrastructure computationnelle qui collecte automatiquement les pages d'accueil de médias québécois, canadiens et américains toutes les 10 minutes depuis 2019. Cette infrastructure permet de mesurer la saillance absolue et relative des objets publics (enjeux, acteurs, institutions) dans l'espace médiatique contemporain.

**§3 - Postdoc + méthodologie:**
> En 2027, il entamera un projet postdoctoral à UCLA sous la supervision du professeur Stuart Soroka, intitulé *"Fox vs CNN: A Longitudinal Analysis of Media Salience and Polarization in the United States"*. Ce projet analysera l'évolution de la polarisation médiatique américaine entre 2019 et 2027 à partir des données Radar+. Ses travaux s'appuient sur R, l'intelligence artificielle (LLM), et les principes de science ouverte et de reproductibilité.

**Contenu EN (traduction équivalente):**

**§1 - Academic bio:**
> Adrien Cloutier is a PhD candidate in Political Science at Université Laval (defense scheduled Fall 2026), where his research focuses on political communication, media agenda, and computational methods. He has been a lecturer since 2024, teaching digital tools and quantitative methodology in social sciences.

**§2 - Dissertation:**
> His dissertation, titled *"Breaking News: Radar+ for Measuring Media Salience in the Digital Age"*, develops a computational infrastructure that automatically collects homepages from Quebec, Canadian, and American media outlets every 10 minutes since 2019. This infrastructure measures the absolute and relative salience of public objects (issues, actors, institutions) in the contemporary media space.

**§3 - Postdoc + methodology:**
> In 2027, he will begin a postdoctoral project at UCLA under the supervision of Professor Stuart Soroka, titled *"Fox vs CNN: A Longitudinal Analysis of Media Salience and Polarization in the United States"*. This project will analyze the evolution of American media polarization between 2019 and 2027 using Radar+ data. His work relies on R, artificial intelligence (LLM), and principles of open science and reproducibility.

**Liens:**
- Google Scholar: https://scholar.google.com/citations?user=RXAdvoMAAAAJ&hl=fr
- GitHub: https://github.com/AdriClout
- LinkedIn: https://ca.linkedin.com/in/adrien-cloutier-868b8b180

**Design:**
- Paragraphes bien espacés
- Titres clairs (H3 ou H4)
- Liens en boutons ou icônes visibles
- Typographie académique (Crimson Pro + Inter)

---

### 3️⃣ RADAR+ (PAGE DÉDIÉE - CENTRALE)

**Structure:**
```
┌─────────────────────────────────────┐
│              Radar+                 │
│  Infrastructure de mesure de la     │
│      saillance médiatique           │
│                                     │
│ [Présentation synthétique]          │
│                                     │
│ [Encadré: Description technique]    │
│ • Collecte automatisée              │
│ • Médias QC/CA/US                   │
│ • Indices de saillance              │
│                                     │
│ [Rôle dans la recherche]            │
│ • Thèse                             │
│ • Publications                      │
│ • Postdoc                           │
│                                     │
│ [Bouton: Accéder à Radar+]          │
│                                     │
│ [Visuels: schémas, cartes]          │
└─────────────────────────────────────┘
```

**Contenu FR:**

**Introduction (2-3 phrases):**
> Radar+ est une infrastructure computationnelle développée entièrement en R pour mesurer la saillance des objets publics dans les médias québécois, canadiens et américains. Le système collecte automatiquement les pages d'accueil de ~20 médias toutes les 10 minutes depuis 2019 et utilise un modèle de langage local (LLM) pour identifier et classifier les objets médiatiques.

**Description technique (encadré):**

**Caractéristiques:**
- **Collecte automatisée:** Toutes les 10 minutes, 24h/24, depuis 2019
- **Sources:** ~20 médias (Le Devoir, La Presse, Globe and Mail, New York Times, Fox News, CNN, etc.)
- **Technologie:** Infrastructure complète en R, base de données relationnelle
- **Intelligence artificielle:** LLM local pour extraction d'entités et classification
- **Indices développés:** Saillance absolue et saillance relative (échelle 0-100)

**Rôle dans la recherche:**

**Thèse doctorale:**
> Radar+ constitue le cœur empirique de ma thèse. L'infrastructure permet d'analyser l'évolution de l'agenda médiatique sur plusieurs années et de mesurer la saillance comparative des objets publics.

**Publications:**
> Les données Radar+ alimentent plusieurs publications sur la saillance médiatique, l'agenda-setting et la communication politique. (→ voir section Publications)

**Projet postdoctoral (UCLA 2027):**
> Radar+ sera utilisé pour analyser la polarisation médiatique entre Fox News et CNN (2019-2027), développer un indice de divergence/convergence, et mesurer l'impact sur l'opinion publique.

**Lien:**
- [Bouton CTA] Accéder à Radar+ → https://www.clessn.com/radar/index.html

**Contenu EN (traduction équivalente):**

**Introduction:**
> Radar+ is a computational infrastructure developed entirely in R to measure the salience of public objects in Quebec, Canadian, and American media. The system automatically collects homepages from ~20 media outlets every 10 minutes since 2019 and uses a local language model (LLM) to identify and classify media objects.

**Technical description (box):**

**Features:**
- **Automated collection:** Every 10 minutes, 24/7, since 2019
- **Sources:** ~20 media outlets (Le Devoir, La Presse, Globe and Mail, New York Times, Fox News, CNN, etc.)
- **Technology:** Complete infrastructure in R, relational database
- **Artificial intelligence:** Local LLM for entity extraction and classification
- **Developed indices:** Absolute and relative salience (scale 0-100)

**Role in research:**

**Doctoral dissertation:**
> Radar+ constitutes the empirical core of my dissertation. The infrastructure allows analyzing the evolution of the media agenda over several years and measuring the comparative salience of public objects.

**Publications:**
> Radar+ data feeds several publications on media salience, agenda-setting, and political communication. (→ see Publications section)

**Postdoctoral project (UCLA 2027):**
> Radar+ will be used to analyze media polarization between Fox News and CNN (2019-2027), develop a divergence/convergence index, and measure impact on public opinion.

**Link:**
- [CTA Button] Access Radar+ → https://www.clessn.com/radar/index.html

**Design:**
- Page dédiée, central dans la navigation
- Encadrés visuels pour description technique
- Schémas/cartes sobres si disponibles
- Bouton CTA très visible
- Visuels: possibilité d'ajouter schéma de l'infrastructure (collecte → traitement → indices)

---

### 4️⃣ EIOM (PAGE DÉDIÉE - ESSENTIELLE)

**Structure:**
```
┌─────────────────────────────────────┐
│              EIOM                   │
│  École interdisciplinaire outils    │
│          & méthodes                 │
│                                     │
│ [Intro: rôle co-créateur]           │
│                                     │
│ [Encadré: Présentation]             │
│                                     │
│ [Objectifs pédagogiques]            │
│                                     │
│ [Format et public cible]            │
│                                     │
│ [Bouton: Visiter EIOM]              │
└─────────────────────────────────────┘
```

**Contenu FR:**

**Introduction (1-2 phrases):**
> Adrien Cloutier est co-créateur et co-organisateur de l'École interdisciplinaire outils & méthodes (EIOM), une école d'été annuelle dédiée aux meilleures pratiques en recherche.

---

**PRÉSENTATION (encadré):**

**École d'été annuelle | Université Laval**

L'**EIOM** est une école d'été interdisciplinaire que j'ai co-créée pour réunir chaque année étudiants, chercheurs et professionnels autour des meilleures pratiques en recherche. L'école offre une formation intensive d'une semaine sur les outils numériques, les méthodes computationnelles et les principes de science ouverte.

**Site web:** https://eiom.ca

---

**OBJECTIFS PÉDAGOGIQUES:**

- **Former aux outils numériques contemporains** (R, Python, Git, LaTeX, etc.)
- **Diffuser les meilleures pratiques méthodologiques** en recherche quantitative et qualitative
- **Favoriser l'interdisciplinarité** et les échanges entre disciplines (sciences sociales, sciences de la santé, sciences naturelles, etc.)
- **Promouvoir la science ouverte** et la reproductibilité des analyses
- **Créer une communauté de pratique** pérenne autour des méthodes et outils de recherche

---

**FORMAT ET PUBLIC CIBLE:**

**Format:**
- École intensive d'une semaine
- Ateliers pratiques et hands-on
- Sessions interactives avec formateurs experts
- Matériel ouvert et code reproductible

**Public cible:**
- Étudiants aux cycles supérieurs (maîtrise et doctorat)
- Chercheurs et chercheurs postdoctoraux
- Professionnels de la recherche
- Toute personne souhaitant améliorer ses compétences méthodologiques

---

**Impact:**

Depuis sa création, l'EIOM a formé des centaines de participants provenant de diverses disciplines et institutions. L'école contribue au développement des compétences méthodologiques et à la diffusion de la culture de science ouverte dans la communauté francophone.

---

**Lien:**
- **[Bouton CTA]** Visiter le site de l'EIOM → https://eiom.ca

---

**Contenu EN:**

**Introduction:**
> Adrien Cloutier is co-creator and co-organizer of the École interdisciplinaire outils & méthodes (EIOM), an annual summer school dedicated to research best practices.

---

**PRESENTATION (box):**

**Annual summer school | Université Laval**

**EIOM** is an interdisciplinary summer school I co-created to bring together students, researchers, and professionals each year around research best practices. The school offers intensive one-week training on digital tools, computational methods, and open science principles.

**Website:** https://eiom.ca

---

**PEDAGOGICAL OBJECTIVES:**

- **Train in contemporary digital tools** (R, Python, Git, LaTeX, etc.)
- **Disseminate methodological best practices** in quantitative and qualitative research
- **Foster interdisciplinarity** and exchanges between disciplines (social sciences, health sciences, natural sciences, etc.)
- **Promote open science** and analysis reproducibility
- **Create a lasting community of practice** around research methods and tools

---

**FORMAT AND TARGET AUDIENCE:**

**Format:**
- Intensive one-week school
- Practical hands-on workshops
- Interactive sessions with expert instructors
- Open materials and reproducible code

**Target audience:**
- Graduate students (Master's and PhD)
- Researchers and postdoctoral researchers
- Research professionals
- Anyone wishing to improve their methodological skills

---

**Impact:**

Since its creation, EIOM has trained hundreds of participants from diverse disciplines and institutions. The school contributes to developing methodological competencies and disseminating the culture of open science in the Francophone community.

---

**Link:**
- **[CTA Button]** Visit EIOM website → https://eiom.ca

---

**Design:**
- Page dédiée (importance de l'EIOM comme réalisation majeure)
- Encadré visuel pour présentation
- Listes claires pour objectifs et format
- Bouton CTA très visible vers https://eiom.ca
- Ton académique mais accessible

---

### 5️⃣ PUBLICATIONS (SIMPLIFIÉ AVEC CATÉGORIES)

**Structure:**
```
┌─────────────────────────────────────┐
│          Publications               │
│                                     │
│ [Bouton très visible: Google Scholar]│
│                                     │
│ ── Articles évalués par les pairs ──│
│ [Liste courte]                      │
│                                     │
│ ── Autres publications ──           │
│ [Liste courte]                      │
│                                     │
│ ── Communications scientifiques ──  │
│ [Liste courte]                      │
└─────────────────────────────────────┘
```

**Contenu FR:**

**Introduction (1 phrase):**
> Mes travaux de recherche portent sur la communication politique, l'agenda médiatique, la polarisation et les méthodes computationnelles.

**Bouton Google Scholar (très visible):**
- [BOUTON LARGE] Google Scholar → https://scholar.google.com/citations?user=RXAdvoMAAAAJ&hl=fr

**Catégories:**

**Articles évalués par les pairs:**
- [Liste à compléter depuis le CV ou laisser placeholder]
- Ou texte: "Liste complète disponible sur Google Scholar"

**Autres publications / rapports:**
- [Placeholder ou liste courte]

**Communications scientifiques:**
- [Placeholder ou liste courte des conférences académiques: SPSA, ACSP, etc.]

**Note:**
> Pour une liste exhaustive et mise à jour, consultez mon profil Google Scholar.

**Contenu EN (traduction):**

**Introduction:**
> My research focuses on political communication, media agenda, polarization, and computational methods.

**Google Scholar button:**
- [LARGE BUTTON] Google Scholar → https://scholar.google.com/citations?user=RXAdvoMAAAAJ&hl=en

**Categories:**

**Peer-reviewed articles:**
- [List from CV or placeholder]
- Or text: "Full list available on Google Scholar"

**Other publications / reports:**
- [Placeholder or short list]

**Conference presentations:**
- [Placeholder or short list: SPSA, CPSA, etc.]

**Note:**
> For a comprehensive and updated list, visit my Google Scholar profile.

**Design:**
- Page très lisible, orientée scan rapide
- Google Scholar button TRÈS visible en haut
- Catégories séparées visuellement (cartes ou sections)
- Listes épurées, pas de surcharge textuelle
- Option: utiliser cards pour chaque catégorie

---

### 6️⃣ ENSEIGNEMENT ET CONFÉRENCES / TEACHING & TALKS

**Structure:**
```
┌─────────────────────────────────────┐
│   Enseignement et conférences       │
│                                     │
│ ─────── ENSEIGNEMENT ───────        │
│                                     │
│ [Carte: POL-6078]                   │
│ [Carte: Méthodologie quantitative]  │
│ [Carte: EIOM]                       │
│                                     │
│ ─────── CONFÉRENCES ─────────       │
│                                     │
│ [Carte: Méthode agile FSS Laval]    │
│ [Structure extensible]              │
└─────────────────────────────────────┘
```

**Contenu FR:**

**ENSEIGNEMENT**

**Carte 1: Outils numériques en sciences sociales**
- **Cours:** POL-6078
- **Institution:** Université Laval
- **Niveau:** Cycles supérieurs (maîtrise/doctorat)
- **Depuis:** 2024
- **Description courte:**
  > Introduction aux outils numériques et méthodes computationnelles pour la recherche en sciences sociales. Le cours couvre R, la visualisation de données, Git, la reproductibilité et l'analyse de texte.
- **Compétences développées:**
  - Autonomie avec R et RStudio
  - Analyses reproductibles
  - Collaboration via Git/GitHub
  - Introduction aux LLM
- **[Lien: Plan de cours]** (ou placeholder: "Disponible sur demande")

**Carte 2: Méthodologie quantitative**
- **Institution:** Université Laval
- **Niveau:** Cycles supérieurs
- **Depuis:** 2024
- **Description courte:**
  > Cours sur les méthodes quantitatives appliquées à la recherche en science politique et sciences sociales. Focus sur l'application rigoureuse des méthodes statistiques et l'interprétation des résultats.
- **Thèmes principaux:**
  - Design de recherche
  - Statistiques descriptives et inférentielles
  - Régression linéaire et logistique
  - Communication des résultats
- **[Lien: Plan de cours]** (ou placeholder)

**Carte 3: EIOM (École interdisciplinaire outils & méthodes)**
- **Rôle:** Co-créateur et co-organisateur
- **Format:** École d'été annuelle
- **Institution:** Université Laval
- **Site web:** https://eiom.ca
- **Description courte:**
  > École d'été interdisciplinaire dédiée aux meilleures pratiques en recherche. Formation intensive d'une semaine sur les outils numériques (R, Python, Git), les méthodes computationnelles et la science ouverte.
- **Public cible:** Étudiants cycles supérieurs, chercheurs, professionnels
- **Objectifs:**
  - Former aux outils numériques contemporains
  - Diffuser les meilleures pratiques méthodologiques
  - Promouvoir la science ouverte et la reproductibilité
  - Créer une communauté de pratique

---

**CONFÉRENCES**

**Carte 1: Utilisation de la méthode agile en milieu académique**
- **Institution:** Faculté des sciences sociales, Université Laval
- **Lien:** https://www.fss.ulaval.ca/evenements/utilisation-de-la-methode-agile-en-milieu-academique
- **Description courte:**
  > Conférence sur l'application des principes de gestion agile (Scrum) à la conduite de projets de recherche et d'enseignement. Partage d'expérience concrète et d'outils pratiques pour structurer efficacement des projets académiques complexes.

**[Structure extensible pour futures conférences]**

---

**Contenu EN (traduction équivalente):**

**TEACHING**

**Card 1: Digital Tools in Social Sciences**
- **Course:** POL-6078
- **Institution:** Université Laval
- **Level:** Graduate (Master's/PhD)
- **Since:** 2024
- **Short description:**
  > Introduction to digital tools and computational methods for social science research. The course covers R, data visualization, Git, reproducibility, and text analysis.
- **Competencies developed:**
  - Autonomy with R and RStudio
  - Reproducible analyses
  - Collaboration via Git/GitHub
  - Introduction to LLMs
- **[Link: Course syllabus]** (or placeholder)

**Card 2: Quantitative Methodology**
- **Institution:** Université Laval
- **Level:** Graduate
- **Since:** 2024
- **Short description:**
  > Course on quantitative methods applied to political science and social science research. Focus on rigorous application of statistical methods and interpretation of results.
- **Main themes:**
  - Research design
  - Descriptive and inferential statistics
  - Linear and logistic regression
  - Communication of results
- **[Link: Course syllabus]** (or placeholder)

**Card 3: EIOM (École interdisciplinaire outils & méthodes)**
- **Role:** Co-creator and co-organizer
- **Format:** Annual summer school
- **Institution:** Université Laval
- **Website:** https://eiom.ca
- **Short description:**
  > Interdisciplinary summer school dedicated to research best practices. Intensive one-week training on digital tools (R, Python, Git), computational methods, and open science.
- **Target audience:** Graduate students, researchers, professionals
- **Objectives:**
  - Train in contemporary digital tools
  - Disseminate methodological best practices
  - Promote open science and reproducibility
  - Create a community of practice

---

**TALKS**

**Card 1: Using Agile Methodology in Academic Settings**
- **Institution:** Faculty of Social Sciences, Université Laval
- **Link:** https://www.fss.ulaval.ca/evenements/utilisation-de-la-methode-agile-en-milieu-academique
- **Short description:**
  > Talk on applying agile management principles (Scrum) to research and teaching project management. Sharing concrete experience and practical tools to effectively structure complex academic projects.

**[Extensible structure for future talks]**

---

**Design:**
- UNE SEULE PAGE regroupée (pas 2 sections séparées)
- Section ENSEIGNEMENT en haut
- Section CONFÉRENCES en bas
- Cartes visuelles pour chaque cours/conférence
- Description courte pour chaque item
- Liens vers plans de cours ou placeholders propres
- Structure extensible (facile d'ajouter futures conférences)

---

### 7️⃣ CAPP / CLESSN (SYNTHÈSE)

**Structure:**
```
┌─────────────────────────────────────┐
│          CAPP / CLESSN              │
│                                     │
│ [Intro: rôle co-coordonnateur]      │
│                                     │
│ ── Centres de recherche ──          │
│ [Carte: CAPP]                       │
│ [Carte: CLESSN]                     │
│                                     │
│ ── Projets liés ──                  │
│ [Carte: Datagotchi]                 │
│ [Carte: Projet Quorum]              │
│ [Carte: Mandats Mitacs]             │
└─────────────────────────────────────┘
```

**Contenu FR:**

**Introduction (1-2 phrases):**
> Adrien Cloutier est co-coordonnateur de deux centres de recherche à l'Université Laval, où il structure des activités, soutient des projets de recherche et contribue au développement d'infrastructures numériques.

---

**CENTRES DE RECHERCHE**

**Carte 1: CAPP (Centre d'analyse des politiques publiques)**
- **Site web:** https://capp-ulaval.ca/
- **Description brève:**
  > Centre de recherche analysant les enjeux de politiques publiques au Québec et au Canada. Le CAPP réunit chercheurs, étudiants et partenaires publics autour de projets appliqués. Adrien y co-coordonne les activités de recherche et contribue à l'articulation entre recherche académique et besoins des décideurs publics.

**Carte 2: CLESSN (Chaire de leadership en enseignement des sciences sociales numériques)**
- **Site web:** https://www.clessn.com/
- **Description brève:**
  > Centre dédié à l'innovation pédagogique et méthodologique en sciences sociales. Le CLESSN développe des outils numériques, forme aux méthodes computationnelles et coordonne des initiatives de recherche collaborative. Adrien y co-coordonne les activités de recherche, notamment le développement de Radar+ et la structuration de projets interdisciplinaires.

---

**PROJETS LIÉS**

**Carte 1: Datagotchi**
- **Site web:** https://www.datagotchi.com/
- **Description brève:**
  > Application ludique et éducative permettant d'explorer les données de manière interactive. Datagotchi vise à rendre les données accessibles au grand public et à favoriser la participation citoyenne à travers la visualisation et l'exploration de données ouvertes.

**Carte 2: Projet Quorum**
- **Site web:** https://www.projetquorum.com/
- **Description brève:**
  > Dispositif de participation publique déployé au Musée de la civilisation permettant aux citoyens de délibérer sur des enjeux publics. Projet Quorum combine recherche en science politique et science citoyenne pour favoriser l'engagement démocratique.

**Carte 3: Mandats de recherche appliquée (Mitacs)**
- **Description brève:**
  > Deux mandats de recherche appliquée au Musée de la civilisation (Mitacs Accélération 2022 et 2024, 15 000 $ chacun). Projets centrés sur l'analyse de données de fréquentation, le développement de dashboards interactifs et la production de rapports d'aide à la décision.
- **Responsabilités:**
  - Nettoyage et intégration de données hétérogènes
  - Analyses longitudinales et modélisation prédictive
  - Scripts R automatisés
  - Formation du personnel
- **Note:** Rapports disponibles sur demande (sous réserve d'autorisation institutionnelle)

---

**Contenu EN (traduction):**

**Introduction:**
> Adrien Cloutier is co-coordinator of two research centers at Université Laval, where he structures activities, supports research projects, and contributes to the development of digital infrastructures.

---

**RESEARCH CENTERS**

**Card 1: CAPP (Public Policy Analysis Center)**
- **Website:** https://capp-ulaval.ca/
- **Brief description:**
  > Research center analyzing public policy issues in Quebec and Canada. CAPP brings together researchers, students, and public partners around applied projects. Adrien co-coordinates research activities and contributes to bridging academic research and the needs of public decision-makers.

**Card 2: CLESSN (Chair in Digital Social Science Leadership)**
- **Website:** https://www.clessn.com/
- **Brief description:**
  > Center dedicated to pedagogical and methodological innovation in social sciences. CLESSN develops digital tools, trains in computational methods, and coordinates collaborative research initiatives. Adrien co-coordinates research activities, including the development of Radar+ and the structuring of interdisciplinary projects.

---

**RELATED PROJECTS**

**Card 1: Datagotchi**
- **Website:** https://www.datagotchi.com/
- **Brief description:**
  > Playful and educational application for exploring data interactively. Datagotchi aims to make data accessible to the general public and foster citizen participation through visualization and exploration of open data.

**Card 2: Projet Quorum**
- **Website:** https://www.projetquorum.com/
- **Brief description:**
  > Public participation device deployed at the Musée de la civilisation allowing citizens to deliberate on public issues. Projet Quorum combines political science research and citizen science to foster democratic engagement.

**Card 3: Applied Research Contracts (Mitacs)**
- **Brief description:**
  > Two applied research contracts at the Musée de la civilisation (Mitacs Accelerate 2022 and 2024, $15,000 each). Projects focused on attendance data analysis, development of interactive dashboards, and production of decision-support reports.
- **Responsibilities:**
  - Data cleaning and integration of heterogeneous databases
  - Longitudinal analyses and predictive modeling
  - Automated R scripts
  - Staff training
- **Note:** Reports available upon request (subject to institutional authorization)

---

**Design:**
- UNE PAGE SYNTHÈSE (pas redondante)
- Section "Centres de recherche" en haut
- Section "Projets liés" en bas (inclut Datagotchi, Quorum, Mitacs)
- Cartes visuelles, pas de longs paragraphes
- Liens vers sites web des centres/projets bien visibles

---

### 8️⃣ RFICS (PAGE DÉDIÉE)

**Structure:**
```
┌─────────────────────────────────────┐
│              RFICS                  │
│  Réseau francophone international   │
│    en conseil scientifique          │
│                                     │
│ [Intro: rôle passé]                 │
│                                     │
│ [Encadré: Faits clés]               │
│                                     │
│ [Responsabilités et réalisations]   │
│                                     │
│ [Impact et portée]                  │
│                                     │
│ [Lien vers RFICS]                   │
└─────────────────────────────────────┘
```

**Contenu FR:**

**Introduction (ton factuel, professionnel):**
> Adrien Cloutier a été coordonnateur scientifique du Réseau francophone international en conseil scientifique (RFICS) de 2022 à 2024. Dans ce rôle, il a piloté les activités de recherche et de développement du réseau et contribué à la structuration de mécanismes de gouvernance collaborative multi-continentale.

---

**FAITS CLÉS (encadré):**

- **Période:** 2022-2024
- **Rôle:** Coordonnateur scientifique
- **Atelier international:** Dakar, Sénégal (11-12 juillet 2024) — Formation sur le conseil scientifique parlementaire
- **Portée géographique:** Amériques, Afrique, Europe
- **Bourse d'excellence RFICS:** 2 000 $ (reconnaissance de la contribution au réseau)

---

**RESPONSABILITÉS ET RÉALISATIONS:**

- **Coordination scientifique:** Pilotage des activités de recherche et développement du réseau (2022-2024)
- **Gouvernance internationale:** Structuration de mécanismes de gouvernance collaborative entre institutions académiques et parlementaires sur trois continents
- **Atelier Dakar (juillet 2024):** Organisation et animation d'un atelier international de formation sur le conseil scientifique parlementaire
- **Partenariats stratégiques:** Développement de partenariats avec institutions académiques et parlementaires en Amériques, Afrique et Europe
- **Livrables stratégiques:** Rédaction de termes de référence pour formations parlementaires sur le conseil scientifique

---

**IMPACT ET PORTÉE:**

- Réseau multi-continental (Amériques, Afrique, Europe)
- Partenariats avec parlements, universités et institutions de recherche
- Formation et renforcement des capacités pour conseillers scientifiques
- Transfert de connaissances entre sphères académique et politique

---

**Lien:**
- **[Bouton]** Site du RFICS (si disponible, sinon retirer)

---

**Contenu EN (traduction):**

**Introduction (factual, professional tone):**
> Adrien Cloutier was scientific coordinator of the Réseau francophone international en conseil scientifique (RFICS) from 2022 to 2024. In this role, he led the network's research and development activities and contributed to structuring collaborative governance mechanisms across multiple continents.

---

**KEY FACTS (box):**

- **Period:** 2022-2024
- **Role:** Scientific Coordinator
- **International workshop:** Dakar, Senegal (July 11-12, 2024) — Training on parliamentary science advice
- **Geographic scope:** Americas, Africa, Europe
- **RFICS Excellence Scholarship:** $2,000 (recognition of contribution to the network)

---

**RESPONSIBILITIES AND ACHIEVEMENTS:**

- **Scientific coordination:** Led research and development activities of the network (2022-2024)
- **International governance:** Structured collaborative governance mechanisms between academic and parliamentary institutions across three continents
- **Dakar workshop (July 2024):** Organized and facilitated an international training workshop on parliamentary science advice
- **Strategic partnerships:** Developed partnerships with academic and parliamentary institutions in the Americas, Africa, and Europe
- **Strategic deliverables:** Drafted terms of reference for parliamentary training on science advice

---

**IMPACT AND REACH:**

- Multi-continental network (Americas, Africa, Europe)
- Partnerships with parliaments, universities, and research institutions
- Training and capacity building for science advisors
- Knowledge transfer between academic and policy spheres

---

**Link:**
- **[Button]** RFICS website (if available)

---

**Design:**
- Page dédiée (importance du rôle passé)
- Ton factuel, professionnel (pas promotionnel)
- Encadré visuel pour "Faits clés"
- Structure claire: Intro → Faits → Responsabilités → Impact
- Bouton vers site RFICS si disponible

---

### 9️⃣ AGILITÉ / NOTION (FUSION OUTILS)

**Structure:**
```
┌─────────────────────────────────────┐
│        Agilité / Notion             │
│  Outils pour la recherche académique│
│                                     │
│ ── Certification Scrum Master ──    │
│ [Carte: Scrum en académie]          │
│                                     │
│ ── Templates Notion ──              │
│ [Grille de cartes: 6 templates]     │
│                                     │
│ [Lien central: notion.com/@adri01]  │
└─────────────────────────────────────┘
```

**Contenu FR:**

**Introduction (1-2 phrases):**
> Adrien Cloutier applique les principes de gestion agile à la conduite de projets de recherche et d'enseignement, et partage une bibliothèque de templates Notion pour organiser la recherche académique.

---

**CERTIFICATION SCRUM MASTER**

**Carte: Approche agile en milieu académique**
- **Certification:** Scrum Master
- **Application:**
  > Adrien applique les principes Scrum à la gestion de projets de recherche et d'enseignement : sprints de rédaction, rétrospectives régulières, backlogs, définition de "done", planification adaptative.
- **Conférence:**
  > "Utilisation de la méthode agile en milieu académique" — Faculté des sciences sociales, Université Laval
  > [Lien] https://www.fss.ulaval.ca/evenements/utilisation-de-la-methode-agile-en-milieu-academique
- **Bénéfices:**
  - Structuration efficace de projets complexes
  - Livraison itérative de résultats
  - Collaboration renforcée
  - Amélioration continue

---

**TEMPLATES NOTION**

**Introduction:**
> Bibliothèque de templates Notion pour organiser la recherche, l'enseignement et les projets académiques. Templates flexibles, modulaires et adaptés aux besoins des chercheurs en sciences sociales.

**Grille de 6 cartes (icônes + titres + descriptions courtes):**

1. **Gestion de thèse**
   - Template complet pour structurer un projet doctoral : planification, revue de littérature, chapitres, timeline, objectifs.

2. **Revue de littérature**
   - Système de gestion de références bibliographiques, notes de lecture, fiches de synthèse et cartographie conceptuelle.

3. **Planification de cours**
   - Template pour organiser un cours universitaire : objectifs, séances, lectures, évaluations, suivi étudiant.

4. **Gestion de projets (Scrum)**
   - Adaptation du framework Scrum pour projets académiques : sprints, backlog, rétrospectives, kanban.

5. **Suivi de publications**
   - Tracker pour gérer le processus de publication : soumissions, révisions, statuts, deadlines, revues ciblées.

6. **Réunions & Notes**
   - Template pour documenter réunions, supervisions, entretiens de recherche avec suivi des actions.

---

**Lien central:**
- **[Bouton CTA]** Accéder aux templates Notion → https://www.notion.com/@adri01

**Note:**
> Certains templates sont en accès public, d'autres sont disponibles sur demande.

---

**Contenu EN (traduction):**

**Introduction:**
> Adrien Cloutier applies agile management principles to research and teaching projects, and shares a library of Notion templates to organize academic research.

---

**SCRUM MASTER CERTIFICATION**

**Card: Agile approach in academic settings**
- **Certification:** Scrum Master
- **Application:**
  > Adrien applies Scrum principles to research and teaching project management: writing sprints, regular retrospectives, backlogs, definition of "done", adaptive planning.
- **Talk:**
  > "Using Agile Methodology in Academic Settings" — Faculty of Social Sciences, Université Laval
  > [Link] https://www.fss.ulaval.ca/evenements/utilisation-de-la-methode-agile-en-milieu-academique
- **Benefits:**
  - Effective structuring of complex projects
  - Iterative delivery of results
  - Enhanced collaboration
  - Continuous improvement

---

**NOTION TEMPLATES**

**Introduction:**
> Library of Notion templates to organize research, teaching, and academic projects. Flexible, modular templates adapted to the needs of social science researchers.

**Grid of 6 cards (icons + titles + short descriptions):**

1. **Dissertation Management**
   - Complete template for structuring a doctoral project: planning, literature review, chapters, timeline, objectives.

2. **Literature Review**
   - Reference management system, reading notes, synthesis sheets, and conceptual mapping.

3. **Course Planning**
   - Template for organizing a university course: objectives, sessions, readings, evaluations, student tracking.

4. **Project Management (Scrum)**
   - Adaptation of the Scrum framework for academic projects: sprints, backlog, retrospectives, kanban.

5. **Publication Tracking**
   - Tracker to manage the publication process: submissions, revisions, statuses, deadlines, targeted journals.

6. **Meetings & Notes**
   - Template for documenting meetings, supervisions, research interviews with action tracking.

---

**Central link:**
- **[CTA Button]** Access Notion templates → https://www.notion.com/@adri01

**Note:**
> Some templates are publicly accessible, others are available upon request.

---

**Design:**
- UNE PAGE OUTILS (fusion Scrum Master + Notion)
- Section Scrum Master en haut (carte avec description + lien conférence)
- Section Templates Notion en bas (grille de 6 cartes)
- Présentation sous forme de cartes / ressources visuelles
- Lien central vers Notion très visible
- Pas de texte long, focus sur les cartes

---

### 🔟 GALERIE / GALLERY (CONSERVÉ)

**Structure:**
```
┌─────────────────────────────────────┐
│            Galerie                  │
│                                     │
│ [Intro: 1 phrase]                   │
│                                     │
│ [Grille 2x2 ou 4 cartes]            │
│ • Terrain / événements              │
│ • RFICS / EIOM                      │
│ • Conférences                       │
│ • Personnel (chat)                  │
└─────────────────────────────────────┘
```

**Contenu FR:**

**Introduction (1 phrase):**
> Quelques moments capturés lors de projets de recherche, d'enseignement, d'événements internationaux et... de supervision de thèse.

---

**Catégories (4 cartes avec placeholders visuels):**

**1. Terrain / événements**
- Photos d'événements de terrain, collaborations, ateliers
- Placeholder: "Photos à venir" ou images si disponibles

**2. RFICS / EIOM**
- Atelier Dakar (juillet 2024)
- Sessions EIOM
- Événements internationaux
- Placeholder: "Photos à venir"

**3. Conférences**
- Conférence FSS Laval (méthode agile)
- Autres présentations
- Placeholder: "Photos à venir"

**4. Personnel**
- Señor Puel (chat), co-chercheur officiel et expert en procrastination académique
- Placeholder: "Photos à venir"

---

**Contenu EN:**

**Introduction:**
> Some moments captured during research projects, teaching, international events, and... dissertation supervision.

---

**Categories (4 cards with visual placeholders):**

**1. Fieldwork / events**
- Photos from fieldwork events, collaborations, workshops
- Placeholder: "Photos coming soon" or images if available

**2. RFICS / EIOM**
- Dakar workshop (July 2024)
- EIOM sessions
- International events
- Placeholder: "Photos coming soon"

**3. Talks**
- FSS Laval talk (agile method)
- Other presentations
- Placeholder: "Photos coming soon"

**4. Personal**
- Señor Puel (cat), official co-researcher and expert in academic procrastination
- Placeholder: "Photos coming soon"

---

**Design:**
- Galerie visuelle RESPIRABLE
- Grille responsive (2x2 sur desktop, 1 colonne sur mobile)
- Légendes sobres sous chaque image
- AUCUN texte long
- Placeholders élégants si photos pas encore ajoutées

---

### 1️⃣1️⃣ CV (SIMPLIFIÉ)

**Structure:**
```
┌─────────────────────────────────────┐
│               CV                    │
│                                     │
│ [Intro: 1 phrase]                   │
│                                     │
│ [Bouton: CV Français (PDF)]         │
│ [Bouton: CV English (PDF)]          │
│                                     │
│ [Optionnel: Résumé HTML court]      │
└─────────────────────────────────────┘
```

**Contenu FR:**

**Introduction:**
> Téléchargez mon curriculum vitae complet en français ou en anglais.

**Boutons:**
- **[BOUTON LARGE]** CV Français (PDF) → cv/Français/CloutierAdrien_CV_3pages.pdf
- **[BOUTON LARGE]** CV English (PDF) → cv/Anglais/CloutierAdrien_CV_english.pdf

**Optionnel: Résumé HTML court (si souhaité):**
- Formations (3-4 items max)
- Publications principales (3-4 items max)
- Bourses principales (3-4 items max)
- Note: "CV complet disponible en PDF ci-dessus"

---

**Contenu EN:**

**Introduction:**
> Download my complete curriculum vitae in French or English.

**Buttons:**
- **[LARGE BUTTON]** CV Français (PDF) → cv/Français/CloutierAdrien_CV_3pages.pdf
- **[LARGE BUTTON]** CV English (PDF) → cv/Anglais/CloutierAdrien_CV_english.pdf

**Optional: Short HTML summary (if desired):**
- Education (3-4 items max)
- Main publications (3-4 items max)
- Main scholarships (3-4 items max)
- Note: "Full CV available in PDF above"

---

**Design:**
- Page SIMPLE
- Deux boutons bien visibles
- Optionnel: résumé académique très court en HTML (pour SEO)
- Pas de "Téléchargements" séparé — tout est ici

---

### 1️⃣2️⃣ CONTACT (SIMPLIFIÉ)

**Structure:**
```
┌─────────────────────────────────────┐
│            Contact                  │
│                                     │
│ [Email institutionnel très visible] │
│                                     │
│ [Formulaire simple]                 │
│ • Nom                               │
│ • Email                             │
│ • Message                           │
│ • [Bouton Envoyer]                  │
│                                     │
│ [Liens professionnels]              │
│ • Twitter                           │
│ • Google Scholar                    │
│ • GitHub                            │
│ • LinkedIn                          │
└─────────────────────────────────────┘
```

**Contenu FR:**

**Introduction:**
> N'hésitez pas à me contacter pour toute question concernant mes recherches, mon enseignement, ou pour des opportunités de collaboration.

**Email institutionnel (très visible):**
- **ADCLO2@ulaval.ca**

**Formulaire simple:**
- Champ: Nom
- Champ: Email
- Champ: Message (textarea)
- Bouton: Envoyer un email

**Liens professionnels:**
- Twitter: https://twitter.com/CloutierAdrien
- Google Scholar: https://scholar.google.com/citations?user=RXAdvoMAAAAJ&hl=fr
- GitHub: https://github.com/AdriClout
- LinkedIn: https://ca.linkedin.com/in/adrien-cloutier-868b8b180

---

**Contenu EN:**

**Introduction:**
> Feel free to contact me with any questions about my research, teaching, or for collaboration opportunities.

**Institutional email (very visible):**
- **ADCLO2@ulaval.ca**

**Simple form:**
- Field: Name
- Field: Email
- Field: Message (textarea)
- Button: Send email

**Professional links:**
- Twitter: https://twitter.com/CloutierAdrien
- Google Scholar: https://scholar.google.com/citations?user=RXAdvoMAAAAJ&hl=en
- GitHub: https://github.com/AdriClout
- LinkedIn: https://ca.linkedin.com/in/adrien-cloutier-868b8b180

---

**Design:**
- Page SIMPLE
- Email institutionnel très visible en haut
- Formulaire épuré
- Liens professionnels en icônes
- Pas de surcharge

---

## 🎨 GUIDELINES DESIGN (OBLIGATOIRES)

### Style général:
- **Académique, minimal, sobre**
- Beaucoup d'espace blanc
- Typographie claire: Crimson Pro (titres) + Inter (corps)
- Navigation fluide sans surcharge

### Structure de page:
- Cartes pour structurer l'information
- Pages longues MAIS scannables (hiérarchie visuelle forte)
- Sections bien séparées visuellement

### Couleurs:
- Bleu primaire: #2563eb
- Texte: #111827
- Texte secondaire: #6b7280
- Background: #ffffff avec touches de #f9fafb

### Components:
- `.academic-card` pour contenu général
- `.research-center-card` pour centres (bordure gauche colorée)
- `.project-card` pour projets (hover effects)
- Boutons CTA clairs et visibles

### Responsive:
- Desktop: grilles 2 colonnes
- Mobile: 1 colonne, navigation adaptée
- Touch-friendly sur mobile

### INTERDIT:
- Sections redondantes
- Accueil trop textuel (MAX 3-4 lignes)
- Ton marketing / startup
- Multiplication de sous-menus
- Texte long non structuré

---

## ✅ VÉRIFICATION FINALE

### Checklist structure:

- [X] Menu simplifié: 11 sections (pas 12)
- [X] Accueil ultra-épuré (hero + 4 boutons, 3-4 lignes max)
- [X] Toutes les sections existent en FR et EN
- [X] Navigation identique FR/EN
- [X] Aucun contenu perdu (seulement réorganisé)

### Checklist contenu déplacé:

- [X] EIOM: de section dédiée → intégré dans "Enseignement et conférences"
- [X] Mandats Mitacs: de section dédiée → intégré dans "CAPP/CLESSN" (projets liés)
- [X] Postdoc Fox vs CNN: de "Recherche" → intégré dans "À propos"
- [X] Conférences: dispersé → regroupé dans "Enseignement et conférences"
- [X] Téléchargements: section dédiée → fusionné dans "CV" (boutons directs)
- [X] Plans de cours PDFs: "Téléchargements" → liens dans "Enseignement et conférences"
- [X] Rapports Mitacs PDFs: "Téléchargements" → note dans "CAPP/CLESSN"
- [X] Scrum Master: "Outils & Méthodes" → fusionné dans "Agilité / Notion"
- [X] Templates Notion: "Outils & Méthodes" → fusionné dans "Agilité / Notion"

### Checklist design:

- [X] Style académique minimal
- [X] Beaucoup d'espace blanc
- [X] Typographie claire (Crimson Pro + Inter)
- [X] Cartes visuelles pour structurer
- [X] Pages scannables avec hiérarchie forte
- [X] Navigation fluide

### Checklist bilingue:

- [X] Chaque section existe en FR
- [X] Chaque section existe en EN (traduction équivalente)
- [X] Structure identique FR/EN
- [X] Menu traduit correctement

---

## 📦 LIVRABLE FINAL

### Fichiers à modifier:

1. **index.html** (version FR) - Refonte complète des 11 sections
2. **index_en.html** (version EN) - Refonte complète des 11 sections (traductions)
3. **assets/css/custom.css** ou **academic-enhanced.css** - Ajustements design si nécessaire

### Prochaines étapes d'implémentation:

1. Créer nouvelle structure HTML (11 sections)
2. Créer section #1 Accueil ultra-épurée
3. Reconstruire chaque section selon wireframes
4. Appliquer design académique sobre
5. Vérifier responsive
6. Tester navigation
7. Dupliquer en anglais (index_en.html)
8. Commit final

---

## 🎯 RÉSUMÉ DES CHANGEMENTS

**DE 12 SECTIONS → À 12 SECTIONS (restructurées):**

| Ancien | → | Nouveau |
|--------|---|---------|
| (aucun) | → | 1. Accueil (NOUVEAU - ultra-épuré) |
| 1. À propos | → | 2. À propos (restructuré + postdoc) |
| 2. Recherche | → | 3. Radar+ (PAGE DÉDIÉE extraite) |
| 5. EIOM | → | 4. EIOM (PAGE DÉDIÉE - conservée, essentielle) |
| 3. Publications | → | 5. Publications (avec catégories) |
| 4. Enseignement + conférences | → | 6. Enseignement et conférences |
| 7. CLESSN/CAPP + 8. Mandats | → | 7. CAPP / CLESSN (FUSION, ordre inversé) |
| 6. RFICS | → | 8. RFICS (conservé) |
| 9. Outils & Méthodes | → | 9. Agilité / Notion (focus agile + Notion) |
| 10. Galerie | → | 10. Galerie (conservé) |
| 11. Téléchargements | → | 11. CV (fusionné, boutons directs) |
| 12. Contact | → | 12. Contact (simplifié) |

**Contenu réorganisé mais AUCUN contenu perdu! ✅**

---

**FIN DU PLAN DE REFONTE**
