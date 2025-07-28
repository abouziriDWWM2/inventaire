# Inventaire de Courses

Une application web responsive pour gérer votre inventaire de courses avec des fonctionnalités CRUD complètes, des alertes de rupture de stock et des suggestions d'achat intelligentes.

## URL de déploiement

L'application est déployée et accessible à l'adresse : https://inventaireb.netlify.app/

## Fonctionnalités

### ✅ Fonctionnalités CRUD

- **Créer** : Ajouter de nouveaux articles avec nom, quantité, unité et seuil d'alerte
- **Lire** : Afficher tous les articles avec leurs détails et statuts
- **Mettre à jour** : Modifier les informations des articles existants
- **Supprimer** : Retirer des articles de l'inventaire avec confirmation

### 🔴 Gestion des ruptures de stock

- Affichage en rouge des articles en rupture de stock (quantité = 0)
- Affichage en orange des articles avec stock faible (quantité ≤ seuil d'alerte)
- Compteur d'alertes en temps réel

### 💡 Suggestions d'achat

- Suggestions automatiques basées sur les articles en rupture ou stock faible
- Quantités suggérées calculées intelligemment
- Section dédiée qui s'affiche uniquement quand nécessaire

### 🔍 Recherche et filtrage

- Recherche par nom d'article en temps réel
- Filtres par statut : Tous, En stock, Stock faible, Rupture de stock
- Interface intuitive et responsive

### 📱 Design responsive

- Interface adaptée aux mobiles, tablettes et ordinateurs
- Design moderne avec animations fluides
- Notifications toast pour les actions utilisateur

## Technologies utilisées

- **HTML5** : Structure sémantique
- **CSS3** : Styles modernes avec variables CSS et animations
- **JavaScript ES6+** : Logique applicative orientée objet
- **IndexedDB** : Base de données NoSQL côté client pour la persistance

## Structure des données

Chaque article contient :

- `id` : Identifiant unique auto-généré
- `nom` : Nom de l'article
- `quantite` : Quantité actuelle en stock
- `unite` : Unité de mesure (pièces, kg, L, etc.)
- `seuil_alerte` : Quantité minimale avant alerte
- `derniere_date_achat` : Date de dernière modification
- `date_creation` : Date de création de l'article

## Installation et utilisation

1. Clonez ou téléchargez les fichiers
2. Ouvrez `index.html` dans un navigateur moderne
3. Commencez à ajouter vos articles !

## Fonctionnalités avancées

- **Persistance des données** : Toutes les données sont sauvegardées localement dans IndexedDB
- **Gestion d'erreurs** : Messages d'erreur informatifs et gestion des cas limites
- **Interface utilisateur** : Modales pour l'édition et la suppression avec confirmations
- **Notifications** : Système de notifications toast pour les actions réussies/échouées
- **Statistiques** : Affichage du nombre total d'articles et d'alertes

## Compatibilité

Compatible avec tous les navigateurs modernes supportant :

- IndexedDB
- ES6+ JavaScript
- CSS Grid et Flexbox
- Fetch API
