Aless
aless.69
En ligne

lilbthewise — 01/07/2026 13:39
quand je reviens je vous envoie ce que j’ai écrit pour la transcription
lilbthewise — 01/07/2026 13:40
jure????
Aless — 01/07/2026 13:45
j'ai commencé a ecrire mais sah au bout d'un moment c'est fanant
Aless — Hier à 17:21
Envoie le lien de la vidéo btbf elle était banger 
mthds26 — Hier à 19:37
Tiens mon coquin
https://fr.borntobefuck.com/watch/33706
Vittoria - Elle a du Mal à Attendre - Jacquie et Michel TV Vidéo ...
Vittoria - Elle a du Mal à Attendre - Jacquie et Michel TV Vidéo ...
Aless — Hier à 21:05
Mdrrr ta vraiment envoyé en plus 😂
Aless
 a épinglé un message dans ce salon. Voir tous les messages épinglés. — 07:48
torkolocooo — 12:13
L’intervention s’est mal passé
mthds26 — 13:15
# ============================================================
# CHEAT-SHEET DOCKER — Commandes principales
# Aide-mémoire pour débutant sur Docker Desktop
# ============================================================

images:

message.txt
8 Ko
﻿
# ============================================================
# CHEAT-SHEET DOCKER — Commandes principales
# Aide-mémoire pour débutant sur Docker Desktop
# ============================================================

images:
  - commande: "docker images"
    description: "Liste toutes les images présentes sur ta machine"
    exemple: "docker images"

  - commande: "docker pull"
    description: "Télécharge une image depuis Docker Hub (ou un autre registre)"
    exemple: "docker pull nginx:latest"

  - commande: "docker build"
    description: "Construit une image à partir d'un Dockerfile présent dans le dossier"
    exemple: "docker build -t mon-app:1.0 ."

  - commande: "docker tag"
    description: "Ajoute un nom/tag à une image existante (utile avant un push)"
    exemple: "docker tag mon-app:1.0 monuser/mon-app:1.0"

  - commande: "docker push"
    description: "Envoie une image vers un registre (Docker Hub, ACR, etc.)"
    exemple: "docker push monuser/mon-app:1.0"

  - commande: "docker rmi"
    description: "Supprime une ou plusieurs images"
    exemple: "docker rmi mon-app:1.0"

  - commande: "docker history"
    description: "Affiche les couches (layers) qui composent une image"
    exemple: "docker history nginx"

# ============================================================

conteneurs:
  - commande: "docker run"
    description: "Crée et démarre un conteneur à partir d'une image"
    exemple: "docker run -d -p 8080:80 --name mon-nginx nginx"
    options_utiles:
      - "-d          : lance en arrière-plan (detached)"
      - "-p host:conteneur : mappe un port"
      - "--name      : donne un nom au conteneur"
      - "-e VAR=val  : définit une variable d'environnement"
      - "-v          : monte un volume"
      - "--rm        : supprime le conteneur à l'arrêt"
      - "-it         : mode interactif avec terminal"

  - commande: "docker ps"
    description: "Liste les conteneurs en cours d'exécution"
    exemple: "docker ps"

  - commande: "docker ps -a"
    description: "Liste TOUS les conteneurs (même arrêtés)"
    exemple: "docker ps -a"

  - commande: "docker start"
    description: "Démarre un conteneur existant mais arrêté"
    exemple: "docker start mon-nginx"

  - commande: "docker stop"
    description: "Arrête un conteneur en cours d'exécution (arrêt propre)"
    exemple: "docker stop mon-nginx"

  - commande: "docker restart"
    description: "Redémarre un conteneur"
    exemple: "docker restart mon-nginx"

  - commande: "docker rm"
    description: "Supprime un conteneur (doit être arrêté, sauf avec -f)"
    exemple: "docker rm mon-nginx"

  - commande: "docker exec"
    description: "Exécute une commande dans un conteneur déjà lancé (ex: ouvrir un terminal dedans)"
    exemple: "docker exec -it mon-nginx bash"

  - commande: "docker logs"
    description: "Affiche les logs (sorties) d'un conteneur"
    exemple: "docker logs -f mon-nginx"

  - commande: "docker inspect"
    description: "Donne le détail complet (config, réseau, volumes...) d'un conteneur ou image"
    exemple: "docker inspect mon-nginx"

  - commande: "docker stats"
    description: "Affiche en temps réel l'utilisation CPU/RAM des conteneurs actifs"
    exemple: "docker stats"

  - commande: "docker cp"
    description: "Copie un fichier entre ta machine et un conteneur"
    exemple: "docker cp mon-nginx:/etc/nginx/nginx.conf ./nginx.conf"

# ============================================================

volumes:
  - commande: "docker volume create"
    description: "Crée un volume (stockage persistant, survit à la suppression du conteneur)"
    exemple: "docker volume create mon-volume"

  - commande: "docker volume ls"
    description: "Liste les volumes existants"
    exemple: "docker volume ls"

  - commande: "docker volume inspect"
    description: "Détaille un volume (chemin réel sur le disque, etc.)"
    exemple: "docker volume inspect mon-volume"

  - commande: "docker volume rm"
    description: "Supprime un volume"
    exemple: "docker volume rm mon-volume"

# ============================================================

reseaux:
  - commande: "docker network ls"
    description: "Liste les réseaux Docker"
    exemple: "docker network ls"

  - commande: "docker network create"
    description: "Crée un réseau personnalisé (pour faire communiquer plusieurs conteneurs)"
    exemple: "docker network create mon-reseau"

  - commande: "docker network connect"
    description: "Connecte un conteneur existant à un réseau"
    exemple: "docker network connect mon-reseau mon-nginx"

  - commande: "docker network inspect"
    description: "Détaille un réseau (conteneurs connectés, IP, etc.)"
    exemple: "docker network inspect mon-reseau"

# ============================================================

docker_compose:
  - commande: "docker compose up"
    description: "Démarre tous les services définis dans docker-compose.yml"
    exemple: "docker compose up -d"

  - commande: "docker compose down"
    description: "Arrête et supprime les conteneurs/réseaux créés par compose"
    exemple: "docker compose down"

  - commande: "docker compose build"
    description: "Reconstruit les images définies dans docker-compose.yml"
    exemple: "docker compose build"

  - commande: "docker compose logs"
    description: "Affiche les logs de tous les services"
    exemple: "docker compose logs -f"

  - commande: "docker compose ps"
    description: "Liste les services du projet compose en cours"
    exemple: "docker compose ps"

# ============================================================

nettoyage_et_systeme:
  - commande: "docker system df"
    description: "Affiche l'espace disque utilisé par images/conteneurs/volumes"
    exemple: "docker system df"

  - commande: "docker system prune"
    description: "Nettoie tout ce qui n'est pas utilisé (conteneurs arrêtés, images orphelines, cache)"
    exemple: "docker system prune -a"

  - commande: "docker container prune"
    description: "Supprime uniquement les conteneurs arrêtés"
    exemple: "docker container prune"

  - commande: "docker image prune"
    description: "Supprime uniquement les images non utilisées"
    exemple: "docker image prune -a"

  - commande: "docker volume prune"
    description: "Supprime uniquement les volumes non utilisés"
    exemple: "docker volume prune"

  - commande: "docker version"
    description: "Affiche la version de Docker installée"
    exemple: "docker version"

  - commande: "docker info"
    description: "Donne un résumé complet de la configuration Docker locale"
    exemple: "docker info"

# ============================================================

registre_docker_hub:
  - commande: "docker login"
    description: "Connecte ton compte Docker Hub (ou autre registre) en ligne de commande"
    exemple: "docker login"

  - commande: "docker logout"
    description: "Déconnecte ton compte du registre"
    exemple: "docker logout"

  - commande: "docker search"
    description: "Recherche une image sur Docker Hub"
    exemple: "docker search nginx"

# ============================================================
# ASTUCE DÉBUTANT :
# - "docker --help" liste toutes les commandes disponibles
# - "docker <commande> --help" détaille les options d'une commande précise
#   ex: docker run --help
# ============================================================
