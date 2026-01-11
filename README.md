# Générateur de Prompt JSON pour IA (AI JSON Prompt Generator)

![License MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Platform](https://img.shields.io/badge/Platform-Google%20Apps%20Script-green)
![Runtime](https://img.shields.io/badge/Google%20Apps%20Script-V8-green)
![Author](https://img.shields.io/badge/Auteur-Fabrice%20Faucheux-orange)

> **Générez des prompts structurés et complexes pour Midjourney, DALL-E 3 et Stable Diffusion sans écrire une seule ligne de code.**

---

## 📖 Description

Ce projet est une interface web interactive (Single Page Application) conçue pour standardiser la création de prompts pour les IA génératives d'images. Plutôt que de tâtonner avec du langage naturel imprécis, cet outil génère un objet **JSON structuré** contenant tous les paramètres techniques (objectif, éclairage, style) et artistiques.

L'application est **"Client-Side Only"** (toute la logique est dans le navigateur), ce qui la rend extrêmement rapide et facile à héberger, que ce soit sur GitHub Pages ou via Google Apps Script.

### 🎯 Pourquoi utiliser le format JSON pour les prompts ?
* **Précision** : Sépare clairement le sujet, l'action et le style technique.
* **Reproductibilité** : Permet de réutiliser des configurations techniques (ex: un setup caméra spécifique) sur différents sujets.
* **Compatibilité** : Optimisé pour les modèles récents (Midjourney v6, Flux, DALL-E 3) qui interprètent de mieux en mieux les structures de données.

---

## ✨ Fonctionnalités Clés

| Catégorie | Détails |
| :--- | :--- |
| **4 Modes Dédiés** | `👤 Portrait` (Humain), `🐾 Animal` (Faune), `🏔️ Paysage` (Environnement), `📦 Objet` (Packshot). |
| **UX/UI Moderne** | Interface fluide construite avec **Tailwind CSS**, totalement responsive (Mobile & Desktop). |
| **Photographie Virtuelle** | Simulation précise d'objectifs (16mm, 85mm...), d'ouvertures (f/1.8, f/8) et de pellicules (Kodak Portra, Fujifilm). |
| **Traduction Auto** | Les champs de sélection sont en Français pour l'utilisateur, mais le JSON généré est en **Anglais** pour l'IA. |
| **Syntax Highlighting** | Visualisation en temps réel du code JSON généré avec coloration syntaxique. |

---

## 📂 Structure du Projet

```text
gemini_prompt_banana_json/
├── Code.gs          # Script Backend (uniquement pour déploiement Google Apps Script)
├── Index.html       # L'application complète (HTML + CSS + JS Logique)
├── LICENSE          # Licence MIT
└── README.md        # Documentation du projet
