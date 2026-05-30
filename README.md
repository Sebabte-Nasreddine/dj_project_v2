# Application e-commerce Django avec Authentification et Docker

Application e-commerce Django containerisée avec Docker, MySQL et prête pour déploiement cloud avec Dokploy.

## Fonctionnalités



## Déploiement sur Dokploy

### 1. Préparer l'image Docker

Construire et pousser l'image vers Docker Hub:
```bash
# Remplacer "username" par votre nom d'utilisateur Docker
docker build -t username/mon-projet-django:v1 .
docker login
docker push username/mon-projet-django:v1
```

### 2. Accéder à Dokploy

- URL: http://IP_VM:3000


### 3. Créer le projet et le service



### 4. Configurer Docker Compose



### 5. Configurer les variables d'environnement

Dans l'onglet **Environment**, ajouter:
```
DJANGO_SECRET_KEY=change-this-secret-key
DJANGO_DEBUG=1
DJANGO_ALLOWED_HOSTS=*
MYSQL_ROOT_PASSWORD=root
MYSQL_DATABASE=DB_ECOMMERCE
MYSQL_USER=django
MYSQL_PASSWORD=django
MYSQL_HOST=db
MYSQL_PORT=3306
```


## Variables d'environnement importantes

| Variable | Défaut | Description |
|---|---|---|
| `DJANGO_SECRET_KEY` | dev-secret-key | Clé secrète Django (À CHANGER EN PRODUCTION) |
| `DJANGO_DEBUG` | 1 | Mode debug (1 pour dev, 0 pour prod) |
| `DJANGO_ALLOWED_HOSTS` | localhost,127.0.0.1 | Hosts autorisés |
| `MYSQL_DATABASE` | DB_ECOMMERCE | Nom base de données |
| `MYSQL_USER` | django | Utilisateur MySQL |
| `MYSQL_PASSWORD` | django | Mot de passe MySQL |
| `MYSQL_HOST` | db | Host MySQL |

---

**Créé pour déploiement cloud via Dokploy**
