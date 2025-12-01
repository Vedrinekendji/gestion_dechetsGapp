# Application de Gestion des Dépôts d'Ordure – Économie Circulaire

Cette application est une plateforme numérique destinée à améliorer la gestion des dépôts d’ordures dans les quartiers, en impliquant directement les **citoyens** et les **sociétés de collecte/recyclage** représentées par les **administrateurs**.
Elle permet de **signaler, suivre et traiter** efficacement les dépôts grâce à un système de capture d’images/vidéos et un tableau de bord interactif.

---

##  Objectifs du projet

* Réduire les dépôts sauvages d’ordures.
* Permettre aux citoyens de signaler rapidement un dépôt via une **photo ou une vidéo**.
* Offrir aux administrateurs (ISACAM et autres sociétés de tri) un outil centralisé pour **gérer les signalements**, **confirmer les dépôts**, **suivre l’état du traitement** et optimiser leurs interventions.
* Assurer une traçabilité complète du cycle de traitement des déchets.

---

## Les acteurs du système

### 1️ **Citoyens**

* Créent un compte et se connectent à la plateforme.
* Filment un dépôt ou prennent une photo.
* Soumettent une **signalisation** dans l’application.
* Accèdent à leur tableau de bord pour :

  * suivre l’état de leur signalisation,
  * voir si le dépôt a été confirmé,
  * vérifier si le dépôt a été traité.

### 2️ **Administrateurs / Société de tri (HYSACAM)**

* Se connectent au back-office.
* Consultent les signalements envoyés par les citoyens.
* Confirment ou rejettent une signalisation.
* Gèrent le traitement du dépôt :

  * suivi du statut,
  * intervention,
  * clôture du dossier.
* Accèdent à un tableau de bord complet pour visualiser :

  * le nombre de dépôts signalés,
  * les dépôts en cours de traitement,
  * les dépôts déjà nettoyés.

---

##  Fonctionnalités clés

###  Côté Citoyen

* Inscription / Connexion
* Signalisation d'un dépôt (photo/vidéo + description)
* Suivi en temps réel de l’état de la requête
* Tableau de bord personnel

###  Côté Administrateur (ISACAM)

* Gestion des citoyens et des signalements
* Confirmation et traitement des dépôts
* Suivi de l’historique des interventions
* Tableau de bord analytique
* Mise à jour des statuts : *en attente*, *confirmé*, *en traitement*, *terminé*

###  Système global

* Centralisation des informations sur les dépôts
* Gestion automatisée des statuts et des notifications
* Historique et traçabilité complète

---

##  Technologies utilisées

###  **Laravel**

Framework backend en PHP.
Il gère :

* l’API,
* la logique métier,
* la sécurité (authentification),
* la gestion des routes,
* les interactions avec MySQL.

Laravel est choisi pour :

* sa robustesse,
* sa rapidité de développement,
* sa structure très claire pour les applications professionnelles.

---

###  **React + Inertia.js**

Inertia.js permet de connecter **Laravel (backend)** et **React (frontend)** sans créer une API séparée.

* **React** gère l’interface utilisateur moderne, dynamique et responsive.
* **Inertia.js** sert de “pont” entre Laravel et React :

  * pas besoin d’API REST complexe,
  * les pages se chargent rapidement,
  * l’expérience est fluide comme dans une SPA.

Ce choix offre :

* un développement plus simple,
* une meilleure performance,
* un code plus propre et mieux organisé.

---

###  **Filament**

Filament est un outil administratif pour Laravel.
Il permettra de créer très rapidement :

* un tableau de bord admin professionnel,
* la gestion des signalements,
* la gestion des citoyens,
* les statistiques,
* les pages CRUD (Créer, Lire, Modifier, Supprimer).

Il offre :

* un design moderne,
* une interface intuitive pour l’administrateur,
* un gain de temps énorme dans le développement du back-office.

---

###  **Base de données : MySQL**

MySQL stocke toutes les informations du projet :

* utilisateurs,
* signalements,
* photos/vidéos,
* statuts,
* historique des interventions.

Il est performant, stable, et parfaitement compatible avec Laravel via Eloquent ORM.

---

###  **Gestion de version : GitHub**

GitHub est utilisé pour :

* versionner le code,
* sauvegarder l’historique du projet,
* travailler proprement (commits, branches, issues),
* héberger le README et la documentation du projet.

---

## 📁 Architecture simplifiée

```
/app
   /Models
   /Http
/resources
   /js (React + Inertia)
   /views
/database
/public
```

---

##  Vision du projet

Cette application vise à devenir un outil essentiel dans la gestion environnementale urbaine.
Elle renforce l’engagement citoyen tout en facilitant le travail des sociétés de tri comme **HYSACAM**.

Grâce à la digitalisation des signalements, l’efficacité du traitement des dépôts est améliorée, réduisant ainsi l’impact environnemental et les risques sanitaires liés aux dépôts sauvages.

---

##  Statut du projet

En cours de développement (version initiale).

---
