# DevOps Roadmap 2024

## Introduction

Je suis développeur front-end, je souhaite élargir mes compétences en me formant au DevOps. Pour documenter et partager mon apprentissage, j'ai décidé de créer ce dépôt GitHub qui servira à la fois de feuille de route et de ressource pour ceux qui, comme moi, souhaitent faire cette transition.

## Objectif

Fournir une feuille de route structurée pour les développeurs qui souhaitent se lancer dans le DevOps. Je vais y rassembler des ressources, des outils, des bonnes pratiques, et des guides étape par étape pour faciliter cette transition.

## Environnement de Travail

Vous avez deux options principales en fonction de votre configuration actuelle :

1. **Utiliser une Machine Virtuelle (VM) sur Windows ou macOS**  
   Si vous êtes sous Windows ou macOS, vous pouvez utiliser une VM pour émuler un environnement Linux, ce qui vous permettra de suivre les étapes de ce guide dans un environnement similaire à celui utilisé en production.

2. **Utiliser un VPS et se Connecter via SSH**  
   Personnellement, j'utiliserai un VPS (Virtual Private Server) chez Oracle Cloud, auquel je me connecterai via SSH. Cette méthode permet de travailler directement sur un serveur distant, ce qui est souvent la configuration préférée dans le monde DevOps.

### Configuration d'une Machine Virtuelle (VM)

Voici une brève explication pour la configurer :

1. **Télécharger et Installer un Hyperviseur** :  
   Vous aurez besoin d'un logiciel pour créer et gérer des machines virtuelles. Voici deux options populaires :

   - **[VirtualBox](https://www.virtualbox.org/)** : Gratuit et open-source, compatible avec Windows, macOS, et Linux.
   - **[VMware Workstation Player](https://www.vmware.com/products/workstation-player.html)** : Gratuit pour un usage personnel et non commercial.

2. **Télécharger une Image ISO de Linux** :  
   Choisissez une distribution Linux pour installer sur votre VM. Voici quelques-unes des plus populaires :

   - **[Ubuntu](https://ubuntu.com/download/desktop)** : Facile à utiliser, largement supporté.
   - **[Debian](https://www.debian.org/distrib/)** : Connue pour sa stabilité et sa fiabilité.
   - **[CentOS](https://www.centos.org/download/)** : Très stable, souvent utilisé en production.

3. **Créer et Configurer la VM** :

   - Ouvrez VirtualBox ou VMware.
   - Créez une nouvelle VM et attribuez-lui des ressources (RAM, CPU, espace disque).
   - Montez l'image ISO que vous avez téléchargée.
   - Lancez la VM et suivez les instructions pour installer Linux.

4. **Configurer la Connexion SSH** :
   - Une fois Linux installé, vous devrez configurer SSH pour accéder à la VM à distance (ce qui simule un serveur distant).
   - Installez le serveur SSH :
     ```bash
     sudo apt-get install openssh-server
     ```
   - Démarrez le service SSH :
     ```bash
     sudo service ssh start
     ```
   - Notez l'adresse IP de votre VM (vous pouvez la trouver en utilisant `ifconfig` ou `ip addr`).
   - Depuis votre machine hôte, connectez-vous à la VM via SSH :
     ```bash
     ssh user@ip_address
     ```

# 1 - [Linux](./Linux/LINUX.md) 🐧

<!-- Suite...

## 2 - Conteneurisation avec Docker 🐋
2.1 - Introduction à la conteneurisation<br>
2.2 - Installation de Docker<br>
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

## 3 - Gestion de Configuration (Ansible)

## 4 - Cloud (AWS)
Concepts de base : services, réseaux, stockage<br>
Équilibrage de charge (Load balancer) et haute disponibilité<br>
Infrastructure en tant que code (IaC, Terraform)<br>

## 5 - Kubernetes
Concepts de base : pods, services, déploiements<br>
Déploiement et gestion des applications<br>

## 6 - Monitoring et Alerting (Prometeus et Grafana)
Choix des métriques à surveiller<br>
Introduction aux bases de données de séries temporelles (TSDB)<br>
Création de tableaux de bord pour la visualisation des données<br>
Mise en place d’alertes pour les incidents<br>

## 7 - Intégration Continue / Déploiement Continu (CI/CD - Gitlab CI)
Concepts des pipelines d’intégration et de déploiement continu<br>
Mise en place et gestion des pipelines CI/CD<br>
Automatisation des déploiements et des tests<br> 

-->

<!-- ## Structure du Dépôt
Vue d'ensemble de la Feuille de Route :

## Représentation visuelle de la feuille de route DevOps pour 2024, mettant en avant les compétences clés et les outils que je dois apprendre.
Image

## Chemin d'Apprentissage :
Chaque étape sera liée à des tutoriels, articles, vidéos, et projets pratiques que je pourrai suivre pour acquérir une expérience concrète.

## Ressources :
Livres, cours, blogs, et autres ressources pour approfondir ma compréhension du DevOps. -->

<!-- ## Projets et Exercices : -->

## Donnez une étoile! ⭐

J'encourage la collaboration en invitant d'autres personnes à contribuer au dépôt, partager leurs propres expériences, et suggérer des améliorations.
