# Plateforme de Vente aux Enchères Sécurisée

## Description

Ce projet a pour but de concevoir et de développer une **plateforme de vente aux enchères sécurisée**. Il permet à des **vendeurs** de proposer des objets à la vente et à des **acheteurs** de soumettre des offres ou de surenchérir. La plateforme met en place des mécanismes de sécurité robustes pour garantir la **confidentialité** et l'**authentification** des utilisateurs, tout en assurant une interface claire et facile à utiliser.

### Fonctionnalités principales :
- **Côté serveur :**
  - Mise en vente publique d'objets avec confidentialité et authenticité.
  - Collecte et chiffrement des offres des acheteurs.
  - Gestion des enchères et des résultats sécurisés.
  
- **Côté client (vendeur/acheteur) :**
  - Consultation des objets en vente.
  - Participation à des enchères de manière sécurisée.
  - Gestion de l'inscription et de l'authentification avec vérification par email.

- **Côté client malhonnête :**
  - Tester les limites de sécurité pour simuler des attaques et corriger les failles.

## Prérequis

Assurez-vous d'avoir installé **Python 3.x** ainsi que **SQLite** pour la gestion de la base de données.

## Installation et exécution

### Étape 1 : Cloner le projet
```bash

git clone https://github.com/votre-compte/plateforme_encheres.git
cd plateforme_encheres

### Étape 2 : Créer et activer un environnement virtuel

python3 -m venv my-venv
source my-venv/bin/activate

### Étape 3 : Installer les dépendances

pip install -r requirements.txt
### Étape 4 : Créer la base de données

python3 sources/bdd.py
### Un fichier data.db sera créé, contenant les tables users et auctions pour gérer les utilisateurs et les enchères.

### Étape 5 : Lancer le serveur

python3 sources/server.py
Le serveur sera accessible sur 127.0.0.1:6589.

### Étape 6 : Lancer le client

python3 sources/client.py

