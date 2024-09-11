# 2 - Docker 🐋

## Conteneurisation avec Docker

### 2.1 - Introduction à la conteneurisation<br>
La différence entre une architecture monolithique et une architecture de microservices:

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

2.3 - Gestion des images<br>
2.4 - Gestion des réseaux<br>
2.5 - Gestion des stockage<br>
2.6 - Introduction à l'IAC<br>
2.7 - Introduction à l'orchestration avec Swarm<br>
2.8 - Mise en place d'un Registre Privé<br>
2.9 - Build Multistage<br>
2.10 - Sécurité des images Docker<br>
2.11 - Docker dans le Cloud<br>
2.12 - Mini projet<br>
