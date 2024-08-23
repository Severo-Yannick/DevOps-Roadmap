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

# 1 - Linux 🐧

## Tuto Linux complet
Drane académie de Lyon - Cédric Frayssinet :**[Tuto Gnu / Linux - Ubuntu ](https://drane.ac-lyon.fr/spip/IMG/scenari/ubuntuavance/co/Module_Avance.html)** <br>

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

## Les commandes
Commandes dans un terminal linux: **[Commandes de base](https://doc.ubuntu-fr.org/tutoriel/console_commandes_de_base)** <br>
Top des 50 commandes Linux: **[Top 50+ Linux Commands You MUST Know](https://www.digitalocean.com/community/tutorials/linux-commands)** <br>
Les commandes Linux pour débutants: **[The Linux command line for beginners](https://ubuntu.com/tutorials/command-line-for-beginners#1-overview)**

## Editeur de texte VI
Commandes de base VI: **[Basic vi Commands](https://www.cs.colostate.edu/helpdocs/vi.html)** <br>
Utilisation de l'éditeur vi: **[Apprendre à utiliser VI](https://docs.oracle.com/cd/E19620-01/805-1608/6j1io9lha/index.html)** <br>

## Les droits et propriétaires des fichiers
Debian: **[Permissions du système de fichiers](https://www.debian.org/doc/manuals/debian-reference/ch01.fr.html#_filesystem_permissions)** <br>
Wikipedia: **[Permissions UNIX](https://fr.wikipedia.org/wiki/Permissions_UNIX)** <br>
Oracle: **[Droits d'accès aux fichiers et aux répertoires](https://docs.oracle.com/cd/E19620-01/805-1608/6j1io9lh0/index.html)** <br>

## Partitions et gestion des disques
Ubuntu-fr: **[Disques, partitions et systèmes de fichiers](https://doc.ubuntu-fr.org/partitions)** <br>
François Goffinet: **[Disques sous Linux](https://linux.goffinet.org/administration/disques-et-stockage-lvm/disques-linux/)** <br>

## La gestion des utilisateurs
Univ-rennes1: **[Comptes et protection des fichiers](https://perso.univ-rennes1.fr/pierre.nerzic/SYS1A/Amphi%20SYS%202015%20partie%2012%20:%20Utilisateurs.pdf)** <br>
Formatux: **[La gestion des utilisateurs](https://www.formatux.fr/formatux-fondamentaux/module-030-utilisateurs/index.html)** <br>

## La gestion des paquets
Ubuntu-fr: **[Gestionnaire de paquets](https://doc.ubuntu-fr.org/gestionnaire_de_paquets#gestionnaire_de_paquets)** <br>
Ubuntu-fr: **[Le fichier « sources.list »](https://doc.ubuntu-fr.org/sources.list)** <br>
Ubuntu packages: **[Recherche de paquets Ubuntu](https://packages.ubuntu.com/)** <br>
Ubuntu-fr: **[Comment installer un paquet ?](https://doc.ubuntu-fr.org/tutoriel/comment_installer_un_paquet)** <br>

## Interface graphique
MobaXterm: **[Interface graphique qui facilite l'accès aux serveurs et systèmes à distance](https://mobaxterm.mobatek.net/download.html)** <br>

## Serveur SSH
Ubuntu-fr: **[Installation du serveur SSH](https://doc.ubuntu-fr.org/ssh#installation_du_serveur_ssh)** <br>
Ubuntu-fr: **[Utilisation du serveur SSH](https://doc.ubuntu-fr.org/ssh#installation_du_serveur_ssh)** <br>
DigitalOcean (SSH File Transfer Protocol): **[SFTP pour transférer des fichiers en toute sécurité avec un serveur distant](https://www.digitalocean.com/community/tutorials/how-to-use-sftp-to-securely-transfer-files-with-a-remote-server-fr)** <br>
IT-Connect: **[Tunneling SSH](https://www.it-connect.fr/chapitres/tunneling-ssh/)** <br>
DigitalOcean: **[Set Up SSH Keys](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys-on-ubuntu-20-04)** <br>
Ubuntu: **[Configure SSH to use two-factor authentication](https://www.it-connect.fr/chapitres/tunneling-ssh/)** <br>


## Installer un serveur web
Ubuntu-fr: **[Serveur web - LAMP](https://doc.ubuntu-fr.org/lamp)** <br>
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
