# Projet de fin d'études (Bachelier développement d’applications)

## Description
Ce projet est une application de gestion de questionnaires ESG (Environnement, Social et Gouvernance) pour les entreprises. L'application est composée d'un backend développé en Rust et d'un frontend développé en Angular. Elle permet la gestion de la prise de contact entre notre client et ses clients, la gestion des questionnaires, et la génération de statistiques et rapports.

## Fonctionnalités
- Inscription et connexion des utilisateurs
- Gestion des formulaires ESG
- Tableau de bord pour les entreprises
- Système de scoring ESG
- Interface d'administration
- Statistiques et rapports

## Installation

### Backend
1. Cloner le repository backend :
    ```bash
    git clone https://github.com/julien-remmery-vinci/bloc3-PFE-backend.git
    cd bloc3-PFE-backend
    ```

2. Installer les dépendances :
    ```bash
    cargo build
    ```

3. Configurer l'environnement :
    - Renommer le fichier `.env.example` en `.env` et y ajouter les variables suivantes :
        - `DATABASE_URL` : lien de connexion à votre base de données
        - `JWT_SECRET` : secret JWT utilisé pour le chiffrement des tokens d'authentification
        - `HASH_ROUNDS` : nombre de 'rounds' nécessaires au chiffrement des mots de passe avant stockage en base de données

4. Lancer le projet :
    ```bash
    cargo run
    ```

### Frontend
1. Cloner le repository frontend :
    ```bash
    git clone https://github.com/julien-remmery-vinci/bloc3-PFE-frontend.git
    cd bloc3-PFE-frontend
    ```

2. Installer les dépendances :
    ```bash
    npm install
    ```

3. Lancer l'application :
    ```bash
    ng serve
    ```
    L'application sera accessible à l'adresse [http://localhost:4200](http://localhost:4200)

## Utilisation
Pour une expérience optimale, il est recommandé de lancer le frontend et le backend en même temps. Vous pouvez utiliser les requêtes présentes dans le dossier `requests` du backend pour tester l'application sans le frontend.

## Docker
Pour déployer l'application dans un container Docker, utilisez le fichier `Dockerfile` présent dans le dossier backend. Voici les étapes pour construire et lancer le container :

1. Construire l'image Docker :
    ```bash
    docker build -t pfe_backend .
    ```

2. Lancer le container :
    ```bash
    docker run -p 3000:3000 pfe_backend
    ```

## Auteurs
### Backend
- Hadjera Emroska
- Hajar Haouat
- Julien Remmery
- Semih Turkoglu

### Frontend
- Hadjera Emroska
- Hasan Pour Arbastan Nariman
- Hajar Haouat
- Julien Remmery
- Semih Turkoglu
- Zerun Emil

## Remarque
Pour plus de précisions, chaque dossier backend et frontend comporte un README spécifique avec des instructions détaillées.