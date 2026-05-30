# Application e-commerce Django avec Authentification

Application e-commerce Django en ajoutant l'authentification.

## Modifications apportées

### Nouvelle application `accounts` ajoutée
- **Inscription (signup)** : Création de nouveaux comptes utilisateur
- **Connexion (login)** : Authentification des utilisateurs
- **Profil** : Page protégée affichant les informations du compte
- **Déconnexion** : Gestion de la déconnexion

### Fonctionnalités incluses
- Formulaire d'inscription avec validation d'email
- Templates Bootstrap 5 pour l'interface utilisateur
- Authentification basée sur Django Auth
- Navigation responsive avec statut utilisateur
- Redirections intelligentes après login/logout

### Routes disponibles
- `/accounts/signup/` - Page d'inscription
- `/accounts/login/` - Page de connexion
- `/accounts/logout/` - Déconnexion
- `/accounts/profile/` - Profil utilisateur (protégé)
- `/products/` - Liste des produits
- `/products/<id>/` - Détail d'un produit
- `/admin/` - Interface d'administration

### Configuration de base de données
Le projet utilise SQLite pour la simplicité. La base de données est automatiquement créée lors de la première migration.

### Démarrage du serveur
```bash
source env_new/bin/activate
python manage.py runserver
```
