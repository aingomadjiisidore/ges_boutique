# 🛒 Boutique Ali

Une application e-commerce développée avec **Laravel**, permettant la gestion des produits, des clients et des commandes.

---

## 📋 Table des matières

- [Présentation](#présentation)
- [Fonctionnalités](#fonctionnalités)
- [Prérequis](#prérequis)
- [Installation](#installation)
- [Configuration](#configuration)
- [Structure de la base de données](#structure-de-la-base-de-données)
- [Utilisation](#utilisation)
- [Contribution](#contribution)
- [Licence](#licence)

---

## 📌 Présentation

**Boutique Ali** est une plateforme de vente en ligne construite avec le framework Laravel. Elle offre une interface simple et efficace pour gérer un catalogue de produits, suivre les commandes et administrer les clients.

---

## ✅ Fonctionnalités

### 🛍️ Gestion des Produits
- Ajouter, modifier et supprimer des produits
- Gestion des catégories de produits
- Gestion des stocks et des prix
- Upload d'images pour chaque produit

### 👥 Gestion des Clients
- Inscription et connexion des clients
- Profil client avec historique
- Gestion des adresses de livraison

### 📦 Gestion des Commandes
- Création et suivi des commandes
- Statuts de commande (En attente, En cours, Livrée, Annulée)
- Historique des commandes par client
- Génération de factures

---

## 🛠️ Prérequis

Avant de commencer, assurez-vous d'avoir installé :

- **PHP** >= 8.1
- **Composer** >= 2.x
- **Laravel** >= 10.x
- **MySQL** >= 8.0 ou **MariaDB** >= 10.x
- **Node.js** >= 18.x et **NPM**
- **Git**

---

## 🚀 Installation

### 1. Cloner le projet

```bash
git clone https://github.com/votre-utilisateur/boutique-ali.git
cd boutique-ali
```

### 2. Installer les dépendances PHP

```bash
composer install
```

### 3. Installer les dépendances JavaScript

```bash
npm install
npm run build
```

### 4. Copier le fichier d'environnement

```bash
cp .env.example .env
```

### 5. Générer la clé de l'application

```bash
php artisan key:generate
```

### 6. Lancer les migrations et les seeders

```bash
php artisan migrate --seed
```

### 7. Démarrer le serveur de développement

```bash
php artisan serve
```

L'application sera disponible à l'adresse : [http://localhost:8000](http://localhost:8000)

---

## ⚙️ Configuration

Modifiez le fichier `.env` avec vos paramètres :

```env
APP_NAME="Boutique Ali"
APP_ENV=local
APP_DEBUG=true
APP_URL=http://localhost

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=boutique_ali
DB_USERNAME=root
DB_PASSWORD=votre_mot_de_passe
```

---

## 🗄️ Structure de la base de données

### Tables principales

| Table        | Description                          |
|--------------|--------------------------------------|
| `users`      | Comptes utilisateurs / clients       |
| `produits`   | Catalogue des produits               |
| `categories` | Catégories des produits              |
| `commandes`  | En-têtes des commandes               |
| `commande_produit` | Lignes de commande (pivot)     |

### Relations

- Un **client** peut passer plusieurs **commandes**
- Une **commande** peut contenir plusieurs **produits**
- Un **produit** appartient à une **catégorie**

---

## 📂 Structure du projet
---

## 🧪 Tests

Pour exécuter les tests :

```bash
php artisan test
```

---

## 🤝 Contribution

Les contributions sont les bienvenues !

1. Forkez le projet
2. Créez une branche : `git checkout -b feature/ma-fonctionnalite`
3. Commitez vos changements : `git commit -m "Ajout d'une nouvelle fonctionnalité"`
4. Poussez la branche : `git push origin feature/ma-fonctionnalite`
5. Ouvrez une Pull Request

---
## Auteur
Aingomadji isidore
