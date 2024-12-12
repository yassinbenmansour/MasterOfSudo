# Born2beroot

## Table des matières

1. [Qu'est-ce que la virtualisation ?](#virtualisation)
2. [Qu'est-ce qu'une machine virtuelle (VM) ?](#machine-virtuelle)
3. [Différences de base entre Rocky Linux et Debian](#rocky-linux-debian)
4. [AppArmor et apt vs. aptitude](#apparmor-apt-aptitude)
5. [Partitions, objectif et configuration](#partitions)
6. [Comment afficher les partitions de la machine ?](#afficher-partitions)
7. [Qu'est-ce qu'une partition primaire et une partition logique ?](#partition-primaire-logique)
8. [Quelle est la différence entre un volume chiffré et une partition chiffrée ?](#volume-chiffre-partition-chiffre)
9. [Comment fonctionne LVM et de quoi s'agit-il ?](#lvm)
10. [Qu'est-ce que Sudo, pourquoi l'utiliser et comment configurer des règles strictes ?](#sudo)
11. [Comment créer un utilisateur et changer son mot de passe ?](#creer-utilisateur)
12. [Comment créer un groupe et attribuer des utilisateurs à celui-ci ?](#creer-groupe)
13. [Comment imprimer les groupes auxquels appartient un utilisateur ?](#imprimer-groupes)
14. [Comment changer le nom d'hôte de la machine ?](#changer-nom-hote)
15. [Comment configurer une politique de mot de passe stricte ?](#politique-mot-passe)
16. [Les bases de la ligne de commande Linux](#ligne-commande-linux)
17. [Qu'est-ce que SSH, comment ça marche et comment le configurer ?](#ssh)
18. [Qu'est-ce que UFW, comment ça marche et comment le configurer ?](#ufw)
19. [Conseils supplémentaires](#conseils-supplementaires)

## Virtualisation

La virtualisation est une technologie qui permet de créer des versions virtuelles de ressources physiques (serveurs, réseaux, stockage, etc.) pour une utilisation plus efficace et flexible.

## Machine virtuelle

Une machine virtuelle est un environnement isolé qui fonctionne comme un ordinateur autonome.

## Rocky Linux Debian

Rocky Linux est une distribution Linux communautaire hautement compatible avec Red Hat Enterprise Linux (RHEL). Elle offre stabilité, sécurité et support de niveau entreprise.

Debian est une distribution Linux populaire connue pour sa stabilité, sa sécurité et sa large gamme de logiciels.

## AppArmor apt aptitude

AppArmor est un module de sécurité Linux qui restreint les capacités des applications.

apt et aptitude sont tous deux des outils de gestion de paquets pour Debian et les systèmes basés sur Debian.

## Partitions

Les partitions sont des divisions d'un disque dur qui permettent de le traiter comme plusieurs disques logiques.

## Afficher partitions

Vous pouvez utiliser les commandes suivantes pour afficher vos partitions de disque :

* `fdisk -l`
* `lsblk`
* `df -h`

## Partition primaire logique

Partitions primaires : Un disque dur peut avoir jusqu'à quatre partitions primaires.

Partitions logiques : Les partitions étendues peuvent contenir plusieurs partitions logiques.

## Volume chiffré partition chiffrée

Volume chiffré : Un disque entier ou une partition entière est chiffré.

Partition chiffrée : Seules certaines partitions sont chiffrées.

## LVM

LVM (Logical Volume Manager) est une couche logicielle qui gère le stockage sur disque.

## Sudo

Sudo (superuser do) est une commande qui permet aux utilisateurs d'exécuter des commandes avec des privilèges root.

## Créer utilisateur

Pour créer un utilisateur, utilisez la commande `useradd`.

## Créer groupe

Pour créer un groupe, utilisez la commande `groupadd`.

## Imprimer groupes

Utilisez la commande `groups` pour lister les groupes auxquels appartient un utilisateur.

## Changer nom hôte

Modifiez le fichier `/etc/hostname` et le champ `hostname` dans `/etc/hosts`.

## Politique de mot de passe

Vous pouvez utiliser des outils comme `pam-auth-update` ou modifier les fichiers de configuration des modules d'authentification par mot de passe pour appliquer des politiques de mot de passe strictes.

## Ligne de commande Linux

La ligne de commande Linux est une interface puissante pour interagir avec votre système. Les commandes de base incluent :

* `cd` : Changer de répertoire
* `ls` : Lister les fichiers et les répertoires
* `mkdir` : Créer un répertoire
* `rm` : Supprimer des fichiers et des répertoires
* `cp` : Copier des fichiers
* `mv` : Déplacer ou renommer des fichiers
* `cat` : Afficher le contenu d'un fichier
* `less` : Afficher un fichier page par page
* `grep` : Rechercher des modèles dans des fichiers


## SSH

SSH (Secure Shell) est un protocole réseau cryptographique qui permet une communication sécurisée entre deux ordinateurs sur un réseau non sécurisé.

## UFW

UFW (Uncomplicated Firewall) est une application de pare-feu conviviale pour Linux. Il vous permet de configurer facilement des règles de pare-feu pour protéger votre système contre les accès non autorisés.

## Conseils supplémentaires

* Mettez régulièrement à jour votre système : Gardez votre système à jour avec les derniers correctifs de sécurité.
* Utilisez des mots de passe forts : Créez des mots de passe forts et uniques pour tous vos comptes.
* Activez l'authentification à deux facteurs : Cela ajoute une couche de sécurité supplémentaire à vos comptes.
