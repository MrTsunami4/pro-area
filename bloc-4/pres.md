---
marp: true
header: "Concevoir une architecture logicielle"
footer: "Epitech - 2024"
theme: uncover
paginate: true
_paginate: false
---

# Créer une architecture logicielle pour des applications web

---

## Pilotage du développement du front-end

---

### Interfaces graphiques

- Connection à l'application
- Connexion à aux services
- Mise en place des reactions

---

### Interfaces graphiques - accessibilité

- Support du Accessible Rich Internet Applications (ARIA)
- Support de la lecture d'écran native du navigateur ou du téléphone

---

### Interfaces graphiques - justification

- Page unique pour simplifier la navigation
- Gros boutons pour faciliter l'utilisation

---

### Front-end - code opérationnel

- Page principale
- Formulaire de connexion

---

### Front-end - nommage et formatage

- Utilisation de Prettier pour le formatage
- Utilisation de ESLint pour le nommage

---

### Front-end - composants tiers

- Utilisation de React pour la création des composants
- Next.js pour la gestion des routes

---

### Front-end - gestion d'erreur

- Recuperation des codes d'erreur de l'API
- Affichage d'un message d'erreur

---

## Pilotage du développement du back-end

---

### Back-end - code opérationnel

- about.json
- Sign-in et Login

---

### Back-end - gestion des ressources

- Utilisation de la base de données pour stocker les utilisateurs
- Cache pour les sessions et de Next.js
- Front rendu par Next.js pour le web

---

### Back-end - nommage et formatage

- Utilisation de Prettier pour le formatage
- Utilisation de ESLint pour le nommage

---

### Back-end - sécurité

- Utilisation de Lucia auth pour l'authentification
  - Chiffrement des mots de passe
  - Utilisation de JWT pour mobile, et de cookies pour le web

---

### Back-end - gestion d'erreur

- Code 404 pour les ressources non trouvées
- Code 302 pour les redirections si l'utilisateur n'est pas connecté
- Code 500 pour les erreurs serveur
