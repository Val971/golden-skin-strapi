# Golden Skin eCommerce - Backend(Strapi)

Bienvenue sur le dépôt backend de **Golden Skin**, une application de e-commerce de vente de produits de beauté. Ce projet utilise **Strapi** comme système de gestion de contenu (CMS) et est déployé sur Render.

## Table des matières

- [Technologies utilisées](#technologies-utilisées)
- [Fonctionnalités](#fonctionnalités)
- [Prérequis](#prérequis)
- [Installation et configuration](#installation-et-configuration)
- [Utilisation](#utilisation)
- [Déploiement](#déploiement)
- [Variables d'environnement](#variables-denvironnement)
- [API Documentation](#api-documentation)
- [Contributions](#contributions)
- [Licence](#licence)

## Technologies utilisées

- **Strapi** (CMS Headless)
- **PostgreSQL** (Base de données)
- **Cloudinary** (Gestion des médias)
- **Render** (Hébergement du backend)
- **Next.js** (Frontend du site web)
- **Vercel** (Hébergement du frontend)
  
## Fonctionnalités

- **Gestion des produits** : Création, mise à jour, suppression des produits via l'interface admin de Strapi.
- **Intégration de Cloudinary** : Gestion et stockage des images produits.
- **API REST/GraphQL** : Exposition des données produits, catégories, et autres entités sous forme d'API.
- **Authentification et gestion des utilisateurs** : Géré par les plugins Strapi pour sécuriser l'accès aux données sensibles.

## Prérequis

Avant de cloner et d'exécuter cette application, assurez-vous d'avoir installé les outils suivants :

- **Node.js** (Version 14 ou supérieure)
- **npm** ou **yarn**
- **PostgreSQL** (Localement ou via un service comme Render)
- **Cloudinary** (pour la gestion des images)

## Installation et configuration

### 1. Cloner le dépôt

```bash
git clone https://github.com/ton-utilisateur/golden-skin-strapi-backend.git
cd golden-skin-strapi-backend
```

### 2. Installer les dépendances

```bash
npm install
```

### 3. Configurer les variables d'environnement

Créez un fichier `.env` à la racine du projet avec les variables suivantes :

```bash
# Strapi settings
APP_KEYS=your_app_keys_here
API_TOKEN_SALT=your_api_token_salt_here

# Database settings
DATABASE_HOST=your_database_host_here
DATABASE_PORT=5432
DATABASE_NAME=your_database_name_here
DATABASE_USERNAME=your_database_user_here
DATABASE_PASSWORD=your_database_password_here

# Cloudinary settings
CLOUDINARY_NAME=your_cloudinary_name_here
CLOUDINARY_KEY=your_cloudinary_key_here
CLOUDINARY_SECRET=your_cloudinary_secret_here

# Other settings
ADMIN_JWT_SECRET=your_admin_jwt_secret_here
```

### 4. Lancer l'application

```bash
npm run develop
```

L'API sera disponible à l'adresse : `http://localhost:1337`

## Déploiement

### Sur Render

1. Connectez votre dépôt à [Render](https://render.com) et configurez les variables d'environnement via leur interface.
2. Déployez directement en suivant les instructions de Render.

## Variables d'environnement

Les principales variables d'environnement utilisées dans cette application :

- **Database** : Hôte, port, nom de la base de données, nom d'utilisateur, mot de passe.
- **Cloudinary** : Nom, clé API, et secret pour gérer les images.
- **App Keys** : Utilisé pour la sécurité des jetons et des API Strapi.

## API Documentation

La documentation de l'API est générée automatiquement par Strapi et est accessible depuis l'interface d'administration.

- **URL de l'API** : `/api`
- **Documentation** : `/documentation`

## Contributions

Les contributions sont les bienvenues ! Veuillez soumettre une pull request ou ouvrir une issue pour discuter des changements que vous souhaitez apporter.

## Licence

Ce projet est sous licence MIT.

---

Cela devrait te donner une structure claire et professionnelle pour ton projet Strapi lié à **Golden Skin**. Assure-toi d'adapter les variables et les instructions selon tes propres besoins.
