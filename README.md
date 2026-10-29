# 🚌 Système de Gestion du Transport Universitaire (Université de MOKPOKPO)

Ce projet est un **Projet Tutoré Académique** ayant pour objectif la conception et la réalisation d'une application web dynamique permettant de gérer, d'organiser et d'automatiser le réseau de transport de l'**Université de MOKPOKPO**.

---

## 📋 Table des Matières

- [1. Contexte & Problématique](#1-contexte--problématique)
- [2. Solution Proposée & Acteurs](#2-solution-proposée--acteurs)
- [3. Spécifications Fonctionnelles](#3-spécifications-fonctionnelles)
- [4. Exigences Non Fonctionnelles](#4-exigences-non-fonctionnelles)
- [5. Périmètre du Projet](#5-périmètre-du-projet)
- [6. Stack Technique & Outils](#6-stack-technique--outils)
- [7. Livrables Attendus](#7-livrables-attendus)

---

## 1. Contexte & Problématique

* **Contexte :** Projet tutoré académique à l'Université de MOKPOKPO.
* **Problématique :** Comment proposer une solution informatique centralisée et accessible permettant d'optimiser l'organisation du transport universitaire (gestion des lignes, horaires, chauffeurs et billets) à l'Université de MOKPOKPO ?

---

## 2. Solution Proposée & Acteurs

La solution est un site web responsive adapté aux ordinateurs et aux téléphones portables. La plateforme s'articule autour de trois (3) profils d'utilisateurs :

1. **👨‍🎓 Étudiant :** Consultation du réseau, achat et gestion des tickets, suivi de planning.
2. **👨‍✈️ Chauffeur :** Consultation des affectations de bus et des plannings de trajet.
3. **👨‍💼 Administrateur :** Gestion complète de la flotte, des lignes, de la planification et du suivi des ventes.

---

## 3. Spécifications Fonctionnelles

### 👨‍🎓 Espace Étudiant
* **Compte :** Inscription, connexion/déconnexion, modification du profil et réinitialisation de mot de passe.
* **Réseau :** Consultation des lignes, itinéraires et horaires des bus.
* **Billetterie :**
  * Sélection de la ligne.
  * Achat de tickets ou abonnements.
  * Paiement simulé pour la démonstration.
  * Génération d'un pass/ticket avec **QR Code**.
  * Annulation d'un ticket (selon les règles de l'université).
* **Suivi :** Consultation du planning de la semaine et de l'historique des achats.

### 👨‍✈️ Espace Chauffeur
* **Authentification :** Connexion et déconnexion sécurisées.
* **Feuille de route :** Consultation du planning quotidien et hebdomadaire.
* **Trajets :** Affichage des détails des trajets attribués (ligne, horaire, bus affecté).

### 👨‍💼 Espace Administrateur
* **Gestion des ressources (CRUD) :**
  * Bus (ajout, modification, suppression).
  * Chauffeurs (création de comptes, affectation).
  * Lignes, itinéraires et arrêts.
  * Tarifs et horaires.
* **Planification :** Attribution d'un bus et d'un chauffeur à chaque trajet (sans conflit d'horaire).
* **Gestion des comptes & Finances :** Suivi des ventes, gestion des utilisateurs.
* **Communication & Analyse :**
  * Diffusion d'annonces aux étudiants.
  * Statistiques de fréquentation et de revenus.
  * Exportation des rapports au format **PDF** ou **Excel**.

---

## 4. Exigences Non Fonctionnelles

* **Sécurité :** Mots de passe hachés, contrôle d'accès selon le rôle (RBAC), protection contre les injections SQL.
* **Ergonomie :** Interface claire, intuitive et **Responsive Design** (adaptée mobile).
* **Intégrité des données :** Vérification automatique pour éviter la double réservation d'un bus ou d'un chauffeur sur un même créneau horaire.
* **Performance & Disponibilité :** Affichage rapide des pages (< 2s) et fonctionnement stable lors des démonstrations.
* **Compatibilité :** Prise en charge des navigateurs web modernes (Chrome, Firefox, Edge, Safari).

---

## 5. Périmètre du Projet

| Inclus dans le projet (In-Scope) | Exclu du projet (Out-of-Scope) |
| :--- | :--- |
| ✅ Site web responsive (Desktop & Mobile) | ❌ Application mobile native (Play Store / App Store) |
| ✅ 3 espaces (Étudiant, Chauffeur, Admin) | ❌ Vrai paiement Mobile Money / CB (Paiement simulé) |
| ✅ Simulation de paiement + Génération QR Code | ❌ Suivi GPS en temps réel des bus |
| ✅ Exportation de rapports (PDF / Excel) | ❌ Gestion des pannes / carburant / entretien mécanique |
| ✅ Déploiement et démo en environnement local | ❌ Notifications par SMS |

---

## 6. Stack Technique & Outils

* **Éditeur de Code :** [VS Code](https://code.visualstudio.com/)
* **Gestion de Version & Collaboration :** Git & GitHub
* **Base de Données & Environnement :** MySQL / Docker
* **Maquettage & UI/UX :** [Figma](https://www.figma.com/)
* **Modélisation de la Base de Données (MCD) :** [Looping](https://www.looping-mcd.fr/)
* **Diagrammes & Conception :** UML / Merise

---

## 7. Livrables Attendus

1. **Cahier des charges fonctionnel et technique** (Ce document).
2. **Dossier de conception :**
   * Maquettes Figma (Wireframes).
   * Modèle Conceptuel de Données (MCD sous Looping).
   * Diagrammes UML (Cas d'utilisation, Séquence).
3. **Code source du projet** (Hébergé sur GitHub).
4. **Manuel d'utilisation** et rapport de projet tutoré.
5. **Démonstration fonctionnelle local** lors de la soutenance.