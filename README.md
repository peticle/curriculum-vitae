<a id="top"></a>

<div align="center">

<a href="https://github.com/peticle/curriculum-vitae">
    <img src="public/favicon.svg" alt="Icône de parchemin" width="120">
</a>

# Curriculum vitæ - Clément Petignat

Curriculum vitæ de Clément Petignat, ingénieur en informatique HES.

Construit avec **Vue 3**, **TypeScript**, **Vite** et **Sass**.

</div>

---

<details>

<summary>Table des matières</summary>

- [À propos du projet](#à-propos-du-projet)
  - [Technologies](#technologies)
- [Démarrage](#démarrage)
  - [Prérequis](#prérequis)
  - [Installation](#installation)
- [Développement](#développement)
  - [Scripts disponibles](#scripts-disponibles)
  - [Serveur de développement](#serveur-de-développement)
  - [Vérification des types](#vérification-des-types)
  - [Linting](#linting)
  - [Formatage](#formatage)
  - [Build de production](#build-de-production)
- [Structure du projet](#structure-du-projet)
- [Contact](#contact)

</details>

---

## À propos du projet

Ce dépôt contient le code source de mon CV personnel, développé sous forme de Single Page Application (SPA) avec Vue 3 et Vite.

- 👤 Présentation personnelle (à propos)
- 🎓 Formation et études
- 💼 Expériences professionnelles
- 🛠️ Compétences techniques (développement, outils, logiciels, données/IA, infrastructure)
- 🗣️ Compétences linguistiques
- 🎯 Projets personnels et centres d'intérêt

### Technologies

[![Node.js](https://img.shields.io/badge/Node.js-26+-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![Vue.js](https://img.shields.io/badge/Vue.js-3-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white)](https://vuejs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-6.x-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-8-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vite.dev/)
[![Sass](https://img.shields.io/badge/Sass-Embedded-CC6699?style=for-the-badge&logo=sass&logoColor=white)](https://sass-lang.com/)
[![Oxlint](https://img.shields.io/badge/Oxlint-1.83-000000?style=for-the-badge)](https://oxc.rs/docs/guide/usage/linter)
[![Oxfmt](https://img.shields.io/badge/Oxfmt-0.68-000000?style=for-the-badge)](https://oxc.rs/)

<p align="right">(<a href="#top">Haut de page</a>)</p>

---

## Démarrage

### Prérequis

Avant d'installer le projet, assurez-vous d'avoir :

- Node.js **26.8.2** ou plus récent
- npm

### Installation

1. Cloner le dépôt :

   ```sh
   git clone git@github.com:peticle/curriculum-vitae.git
   ```

2. Se placer dans le dossier du projet :

   ```sh
   cd ./curriculum-vitae
   ```

3. Installer les dépendances :

   ```sh
   npm install
   ```

<p align="right">(<a href="#top">Haut de page</a>)</p>

---

## Développement

### Scripts disponibles

| Commande             | Description                                     |
| -------------------- | ----------------------------------------------- |
| `npm run dev`        | Démarre le serveur de développement Vite        |
| `npm run build`      | Vérifie les types puis build l'application      |
| `npm run build-only` | Build l'application sans vérification des types |
| `npm run preview`    | Sert le build de production en local            |
| `npm run type-check` | Vérifie les types TypeScript Vue                |
| `npm run lint`       | Lance Oxlint                                    |
| `npm run lint:fix`   | Lance Oxlint et corrige automatiquement         |
| `npm run fmt`        | Formate le code source avec Oxfmt               |
| `npm run fmt:check`  | Vérifie le formatage sans le modifier           |

### Serveur de développement

Démarrer le serveur local :

```sh
npm run dev
```

L'application est accessible sur le réseau local grâce à l'option `--host` de Vite.

### Vérification des types

```sh
npm run type-check
```

### Linting

```sh
npm run lint
```

Pour corriger automatiquement les problèmes détectés :

```sh
npm run lint:fix
```

### Formatage

Formater les fichiers sources avec Oxfmt :

```sh
npm run fmt
```

Vérifier le formatage sans modifier les fichiers :

```sh
npm run fmt:check
```

### Build de production

Générer le build de production (avec vérification des types) :

```sh
npm run build
```

Prévisualiser le build de production en local :

```sh
npm run preview
```

<p align="right">(<a href="#top">Haut de page</a>)</p>

---

## Structure du projet

```text
.
└── public                        # Assets statiques (favicon, images, etc.)
└── src
    ├── assets                    # Images et icônes
    ├── components                # Composants Vue réutilisables
    ├── styles                    # Architecture SCSS globale
    └── views                     # Vues de l'application
        ├── page                  # Vue de la page principale
        │   ├── about             # Section "À propos" de la page principale
        │   └── experience        # Section "Expériences" de la page principale
        └── layout                # En-tête et pied de page
```

<p align="right">(<a href="#top">Haut de page</a>)</p>

---

## Contact

**Clément Petignat**

📧 clement.petignat@protonmail.com

Dépôt GitHub :

https://github.com/peticle/curriculum-vitae

<p align="right">(<a href="#top">Haut de page</a>)</p>
