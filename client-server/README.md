# Programmation Réseau en Python : Serveurs et Clients TCP et UDP

Ce projet propose des implémentations de serveurs et clients utilisant les protocoles TCP et UDP en Python, permettant d’explorer les concepts fondamentaux de la programmation réseau.

## Table des Matières

- [Serveur et Client TCP](#serveur-et-client-tcp)
- [Serveur et Client UDP](#serveur-et-client-udp)

## Serveur et Client TCP

### Serveur TCP

Le serveur TCP (`simple_server_tcp.py`) est conçu pour gérer plusieurs connexions simultanément grâce à un modèle multithread.

#### Utilisation

Démarrer le serveur TCP :

```sh
python simple_server_tcp.py
```

![Capture d'écran du serveur TCP](images/server_tcp_screenshot.png)

### Client TCP

Le client TCP (`simple_client_tcp.py`) permet de se connecter au serveur, d’envoyer des messages et de recevoir des réponses.

#### Utilisation

Exécuter le client TCP :

```sh
python simple_client_tcp.py
```

![Capture d'écran du client TCP](images/client_tcp_screenshot.png)

## Serveur et Client UDP

### Serveur UDP

Le serveur UDP (`udp_server.py`) illustre la communication sans connexion propre au protocole UDP.

#### Utilisation

Démarrer le serveur UDP :

```sh
python udp_server.py
```

![Capture d'écran du serveur UDP](images/server_udp_screenshot.png)

### Client UDP

Le client UDP (`udp_client.py`) démontre l’envoi et la réception de messages avec un serveur UDP.

#### Utilisation

Exécuter le client UDP :

```sh
python udp_client.py
```

![Capture d'écran du client UDP](images/client_udp_screenshot.png)

---

Ce projet est une introduction pratique aux communications réseau avec Python, illustrant les différences entre les protocoles TCP et UDP.

