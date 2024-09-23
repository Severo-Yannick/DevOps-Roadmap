# 2 - Docker 🐋

## Conteneurisation avec Docker

### 2.1 - Introduction à la conteneurisation<br>
La différence entre une **architecture monolithique** et une **architecture de microservices**:

Une architecture monolithique est un modèle de développement logiciel traditionnel qui utilise une base de code unique pour exécuter plusieurs fonctions métier. Tous les composants logiciels d'un système monolithique sont interdépendants en raison des mécanismes d'échange de données au sein du système. La modification d'une architecture monolithique est contraignante et prend du temps, car de petites modifications ont un impact sur des pans entiers de la base de code. 

À l'inverse, les microservices sont une approche architecturale qui consiste à décomposer le logiciel en petits composants ou services indépendants. Chaque service joue un rôle unique et communique avec les autres services au moyen d'une interface bien définie. Comme ils s'exécutent indépendamment, vous pouvez mettre à jour, modifier, déployer ou mettre à l'échelle chaque service selon vos besoins.

<img src="./images/monolithic-vs-microservice.png" alt="monolithic vs microservice" width="800"/><br>

### 2.2 - Installation de Docker<br>
**Docker CE (Community Edition)** est la version gratuite et open-source.<br>
**Docker EE (Enterprise Edition)** est la version payante avec des fonctionnalités supplémentaires incluant un support premium, des outils avancés de sécurité et de gestion.

Un lab pour s'entrainer:
- **[Labs play with docker](https://labs.play-with-docker.com/)**<br>

Installation de Docker sur une machine locale:
- **[Install Docker Desktop on Linux](https://docs.docker.com/desktop/install/linux-install/)**<br>
- **[Install Docker Desktop on Mac](https://docs.docker.com/desktop/install/mac-install/)**<br>
- **[Install Docker Desktop on Windows](https://docs.docker.com/desktop/install/windows-install/)**<br>

Installation de Docker sur un serveur Linux:
- **[Install Docker Engine on Debian](https://docs.docker.com/engine/install/debian/)**<br>
- **[Install Docker Engine on Ubuntu](https://docs.docker.com/engine/install/ubuntu/)**<br>
- **[Install Docker Engine on CentOS](https://docs.docker.com/engine/install/centos/)**<br>

Installation de Docker sur un serveur Microsoft:
- **[Docker sur Windows](https://learn.microsoft.com/fr-fr/windows/dev-environment/docker/overview)**<br>

Docker Machine est très utile si Docker **n'est pas installé nativement**.
- **[Déployer et gérer vos hôtes docker avec Docker Machine](https://devopssec.fr/article/deployer-gerer-vos-hotes-docker-avec-docker-machine)**<br>

L'installation de Docker sur une plateforme **PaaS** (Platform as a Service) varie en fonction du fournisseur de cloud, maisvoici les options principales :

- **Google Cloud (GCP)** : Google Kubernetes Engine (GKE) pour gérer des conteneurs Docker sur un cluster Kubernetes. GKE est un service managé qui prend en charge Docker et Kubernetes nativement.

- **Amazon Web Services (AWS)** : Amazon Elastic Container Service (ECS) et Amazon Elastic Kubernetes Service (EKS) pour exécuter et gérer des conteneurs Docker sur des clusters ECS ou Kubernetes.

- **Microsoft Azure** : Azure Kubernetes Service (AKS) permet de déployer des conteneurs Docker dans un environnement Kubernetes managé, utiliser Azure App Service pour exécuter directement des conteneurs Docker.

### 2.3 - Gestion des images<br>
Docker workflow:<br>
<img src="./images/docker-workflow.jpg" alt="docker workflow" width="800"/><br>

Anatomie d'une image Docker:<br>
<img src="./images/docker-image-layers.jpg" alt="Anatomie d'une image Docker" width="800"/><br>

Dockerfile qui contient les instructions pour créer une image Docker d'une application Node.js basée sur Alpine<br>
**[Lien du repository Docker](https://github.com/docker/welcome-to-docker/blob/main/Dockerfile)**<br>
<img src="./images/dockerfile.png" alt="dockerfile" width="800"/><br>

Documentation officielle Docker pour créer un Dockerfile:<br>
**[Writing a Dockerfile](https://docs.docker.com/get-started/docker-concepts/building-images/writing-a-dockerfile/)**<br>

Développement d'une application Web Python de base avec docker-compose:<br>
**[Docker Compose Quickstart](https://overcast.blog/build-push-the-docker-image-to-docker-hub-using-github-actions-74f20d47c483)**<br>

Automatiser une mise à jour d'une image docker depuis github vers dockerhub:<br>
**[Build & Push the Docker image to Docker Hub using GitHub Actions](https://docs.docker.com/compose/gettingstarted/)**<br>
<img src="./images/github-workflow.webp" alt="github workflow" width="800"/><br>


### 2.4 - Gestion des réseaux<br>
Docker network:<br>
**[Manage networks. You can use subcommands to create, inspect, list, remove, prune, connect, and disconnect networks](https://docs.docker.com/reference/cli/docker/network/)**<br>
<img src="./images/networking-docker.jpg" alt="networking docker" width="800"/><br>

### 2.5 - Gestion du stockage<br>
Docker storage:<br>
**[Storage - volumes, bind mounts, and tmpfs](https://docs.docker.com/engine/storage/)**<br>
<img src="./images/types-of-mounts-volume.png" alt="types of mounts volume docker" width="800"/><br>

### 2.6 - Introduction à l'IAC<br>
Infrastructure as code Timeline<br>
<img src="./images/infrastructure-as-code-timeline.png" alt="Infrastructure as code Timeline" width="800"/><br>

### 2.7 Docker compose:<br>
<img src="./images/docker-compose-file.png" alt="docker compose file" width="800"/><br>
Convertir un *dockerfile* en *docker-compose*: **[composerize](https://www.composerize.com/)**<br>


### 2.8 - Introduction à l'orchestration avec Swarm<br>
### 2.9 - Mise en place d'un Registre Privé<br>
### 2.10 - Build Multistage<br>
### 2.11 - Sécurité des images Docker<br>
### 2.12 - Docker dans le Cloud<br>
### 2.13 - Mini projet<br>
