# DevOps Roadmap 2024 : De Développeur Front-End à DevOps

## Introduction

Je suis développeur front-end, je souhaite élargir mes compétences en me formant au DevOps. Pour documenter et partager mon apprentissage, j'ai décidé de créer ce dépôt GitHub qui servira à la fois de feuille de route et de ressource pour ceux qui, comme moi, souhaitent faire cette transition.

## Objectif

Fournir une feuille de route structurée pour les développeurs qui souhaitent se lancer dans le DevOps. Je vais y rassembler des ressources, des outils, des bonnes pratiques, et des guides étape par étape pour faciliter cette transition.

# Environnement de Travail

Vous avez deux options principales en fonction de votre configuration actuelle :

1. **Utiliser une Machine Virtuelle (VM) sur Windows ou macOS**  
   Si vous êtes sous Windows ou macOS, vous pouvez utiliser une VM pour émuler un environnement Linux, ce qui vous permettra de suivre les étapes de ce guide dans un environnement similaire à celui utilisé en production.

2. **Utiliser un VPS et se Connecter via SSH**  
   Personnellement, j'utiliserai un VPS (Virtual Private Server) chez Oracle Cloud, auquel je me connecterai via SSH. Cette méthode permet de travailler directement sur un serveur distant, ce qui est souvent la configuration préférée dans le monde DevOps.

## Configuration d'une Machine Virtuelle (VM)

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

# Linux 🐧

## Hiérarchie des répertoires
La structure des répertoires d'un système Linux, également connue sous le nom de Filesystem Hierarchy Standard (FHS), est une structure arborescente définie qui permet d'éviter que les fichiers ne soient dispersés dans tout le système et de les organiser de manière logique et facile à parcourir.

`/`: Root directory, the top level of the file system.<br>
`/home`: User home directories.<br>
`/bin`: Essential binary executables.<br>
`/sbin`: System administration binaries.<br>
`/etc`: Configuration files.<br>
`/var`: Variable data (logs, spool files).<br>
`/usr`: User programs and data.<br>
`/lib`: Shared libraries.<br>
`/tmp`: Temporary files.

Explication rapide en vidéo: **[Linux Directories Explained in 100 Seconds](https://www.youtube.com/watch?v=42iQKuQodW4)** <br>
Documentation FHS redhat: **[File System Hierarchy Standard (FHS)](https://docs.redhat.com/en/documentation/red_hat_enterprise_linux/4/html/reference_guide/s1-filesystem-fhs#s3-filesystem-usr)** <br>
Documentation FHS ubuntu: **[Linux Filesystem Tree Overview](https://help.ubuntu.com/community/LinuxFilesystemTreeOverview)**

## Les commandes en console linux
Commandes dans un terminal linux: **[Commandes de base](https://doc.ubuntu-fr.org/tutoriel/console_commandes_de_base)** <br>
Top des 50 commandes Linux: **[Top 50+ Linux Commands You MUST Know](https://www.digitalocean.com/community/tutorials/linux-commands)** <br>
Les commandes Linux pour débutants: **[The Linux command line for beginners](https://ubuntu.com/tutorials/command-line-for-beginners#1-overview)**

## Editeur de texte VI en console linux
Commandes de base VI: **[Basic vi Commands](https://www.cs.colostate.edu/helpdocs/vi.html)** <br>
Utilisation de l'éditeur vi: **[Apprendre à utiliser VI](https://docs.oracle.com/cd/E19620-01/805-1608/6j1io9lha/index.html)** <br>

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
