---
marp: true
header: "Concevoir une architecture logicielle"
footer: "Epitech - 2024"
theme: uncover
paginate: true
_paginate: false
size: 16:9
---

# Concevoir une architecture logicielle

---

## Veille technologique

---

### Etude comparative

- Utilisation de TypeScript
  - Avantages: Typage, grande communauté, outils de développement, nombreux frameworks
  - Inconvénients: Nouveau langage dans notre formation

---

- Next.js
  - Avantages: Web et Api, support SSR, performance, Sécurité
  - Inconvénients: Contrainte de structure, plutôt récent

---

- React Native
  - Avantages: Même framework que le web, multiplateforme
  - Pas aussi performant que du natif, pas de support pour les nouvelles fonctionnalités

---

### Identification des technologies

- React
  - Support du Accessible Rich Internet Applications (ARIA)
  - Support de la lecture d'écran native du navigateur ou du téléphone

---

- HTML
  - Pas de CSS pour caché les éléments
  - Utilisation des balises sémantiques
  - Balises alt pour les images

---

### Etudes sécurité

- Node JS
  - CVE-2023-4448, permet un DOS à cause d'une annulation de requête
  - CVE-2023-39332, permet de lire des fichiers arbitraires avec certaines configurations

---

### Veille sécurité informatique

- Mise à jour des dépendances
- Utilisation de dépendances populaires
- Utilisation de dépendances maintenues

---

## Prototypage

---

### Prototypes

- Figma

---

### Prototypes - comparatif

- Figma
  - Avantages: Gratuit, facile à utiliser, partage de prototype
  - Inconvénients: Pas de version offline, pas de version gratuite pour les équipes

---

### Architecture

- Frontend et Backend séparés
- Utilisation de TypeScript

---

### Intégration technique

- Utilisation de Docker
- Utilisation de Docker Compose

---

## Résolution de problèmes algorithmiques complexes

### Implémentation de l'architecture

---

### Bonnes pratiques de développement

```ts
export const usernameSchema = z.object({
  username: z.string().min(4).max(31),
  password: z.string().min(6).max(255),
});
```

---

### Organisation du code

- Next.js utilise un système de page dans des dossiers qui porte le nom de la page

---

### Segmentation du code

- Actions et réactions dans des fichiers séparés

---

### Implémentation algorithmique

- Zod pour la validation des données
- Lucia auth pour l'authentification

---

## Définition des modèles de données

---

### Persistance des données

- Sqlite

---

### Persistance des données - comparatif

- Sqlite

  - Avantages: Facile à utiliser, pas de serveur à installer
  - Inconvénients: Pas de support pour les types, pas de support pour les relations

---

- Postgres
  - Avantages: Support des types, support des relations
  - Inconvénients: Plus compliqué à utiliser, nécessite un serveur

---

### Structure des données

```sql
CREATE TABLE "Action" (
    "id" TEXT NOT NULL PRIMARY KEY,
    "name" TEXT NOT NULL,
    "user_id" TEXT NOT NULL
);
```

---

### Structure des données - justifications

- Utilisation de UUID pour les id
- Relation entre les tables pour simplifier les requêtes
