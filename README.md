# api-microservices-magasin
Ce projet GitHub propose une API basée sur des microservices développée en utilisant le framework Nest.js. L'objectif principal de cette API est de fournir des fonctionnalités de gestion d'utilisateurs, de produits et de commandes dans une architecture distribuée et modulaire.

# Fonctionnalités clés:

1. Microservice d'authentification (Auth):
Ce microservice gère les fonctionnalités d'authentification et d'autorisation. Il fournit des mécanismes d'inscription, de connexion et de gestion des jetons d'accès pour les utilisateurs.

2. Microservice d'utilisateurs (User):
Le microservice d'utilisateurs permet de gérer les informations des utilisateurs. Il offre des fonctionnalités telles que la création, la mise à jour, la suppression et la récupération de profils d'utilisateurs, ainsi que la possibilité de rechercher des utilisateurs par différents critères.

3. Microservice de produits (Product):
Ce microservice prend en charge la gestion des produits. Il permet de créer, mettre à jour, supprimer et récupérer des informations sur les produits disponibles. Il offre également la possibilité de rechercher des produits par nom, catégorie, prix, etc.

4. Microservice de commandes (Order):
Le microservice de commandes gère le processus de commande des utilisateurs. Il permet de passer de nouvelles commandes, de suivre l'état des commandes en cours et de consulter l'historique des commandes précédentes.

# Architecture:
Le projet est implémenté en utilisant le modèle d'architecture de microservices. Chaque microservice est développé de manière indépendante, avec son propre code source, base de données et points d'API spécifiques. La communication entre les microservices est réalisée à l'aide du protocole gRPC (google Remote Procedure Call).

# Technologies utilisées:

Nest.js: Framework Node.js hautement évolutif et modulaire utilisé pour développer chaque microservice.
TypeScript: Langage de programmation typé qui améliore la robustesse et la lisibilité du code.
PostgreSQL: Pour stocker les données des utilisateurs, produits et commandes de manière distribuée.
Docker: Pour faciliter le déploiement des bases de données de chaque microservice.

Instructions d'installation:

Clonez le dépôt GitHub sur votre machine locale.
Installez les dépendances de chaque microservice en utilisant `yarn install` ou `yarn`.
Déployez les bases de données de chaque miroservices sauf **auth** en utilisant `docker-compose up --build`.
Démarrez chaque microservice localement pour les tester.
