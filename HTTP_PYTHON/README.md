# Configuration d'un Serveur HTTP Python avec CGI

Ce guide explique comment mettre en place un serveur HTTP simple en Python avec le support de CGI (Common Gateway Interface) pour servir du contenu dynamique.

## Prérequis

- Python 3.x installé
- Un éditeur de texte
- Un terminal ou invite de commande

## Étapes

### Création d'un script CGI (ex: `hello.py`)

1. Ouvrez un éditeur de texte et créez un fichier nommé `hello.py`.
2. Ajoutez le code nécessaire pour générer une réponse HTTP dynamique.

### Rendre le script exécutable

Dans un terminal, accédez au répertoire contenant `hello.py` et exécutez :

```sh
chmod +x hello.py
```

Cela permet au serveur d'exécuter le script CGI.

### Démarrer le serveur HTTP avec CGI

Dans le même répertoire, lancez la commande suivante :

```sh
python3 -m http.server --cgi
```

- `python3 -m http.server` : Démarre un serveur HTTP de base.
- `--cgi` : Active le support des scripts CGI.

Une fois lancé, un message s'affiche confirmant que le serveur tourne, par exemple : `Serving at: http://0.0.0.0:8000`.

### Accéder au script CGI dans le navigateur

Ouvrez un navigateur et saisissez l'URL suivante :

```sh
http://localhost:8000/hello.py
```

Si tout est bien configuré, vous verrez la page **"Hello, World!"** s'afficher.

## Exemple avec gestion des requêtes GET et POST

Ce projet inclut également un serveur HTTP personnalisé qui gère les requêtes GET et POST, traite les paramètres et gère les cookies.

### Démarrer le serveur personnalisé

1. Créez un fichier `web_server.py` avec le code nécessaire.
2. Exécutez la commande suivante :

```sh
python3 web_server.py
```

Une fois lancé, le serveur est accessible depuis votre navigateur.

### Accéder au serveur personnalisé

Dans un navigateur, entrez l’URL suivante :

```sh
http://localhost:8000
```

Vous verrez apparaître le message **"Handling GET request!"**.

### Envoyer une requête POST avec `curl`

Utilisez `curl` pour tester une requête POST vers le serveur :

```sh
curl -X POST http://localhost:8000
```

Vous devriez voir apparaître dans le terminal **"Handling POST request!"**.

---

Ce guide fournit une introduction pratique à l'utilisation des serveurs HTTP et CGI avec Python.

