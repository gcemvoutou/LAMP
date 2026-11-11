# LAMP — Linux, Apache, MariaDB, PHP

![Raspberry Pi OS](https://img.shields.io/badge/Raspberry%20Pi%20OS-Debian%2013-C51A4A?logo=raspberrypi&logoColor=white)
![Apache](https://img.shields.io/badge/Apache-2.4.68-D22128?logo=apache&logoColor=white)
![MariaDB](https://img.shields.io/badge/MariaDB-11.8.6-003545?logo=mariadb&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-8.4.26-777BB4?logo=php&logoColor=white)

## Présentation du projet

Ce TP, réalisé dans le cadre du **BTS SIO option SISR**, consiste à mettre en place un serveur web **LAMP** sur un Raspberry Pi :

- **L**inux : le système d’exploitation (Raspberry Pi OS) ;
- **A**pache : le serveur HTTP ;
- **M**ySQL / MariaDB : le système de gestion de bases de données ;
- **P**HP : le langage de script côté serveur.

Le serveur est ensuite configuré et testé depuis un poste client Windows : analyse du trafic HTTP avec Wireshark, gestion des logs, contrôle des accès, scripts CGI, authentification, serveurs virtuels, passage en HTTPS, puis utilisation et administration de MariaDB (utilisateurs, droits, sauvegarde et restauration).

## Objectifs

- Installer et vérifier une pile LAMP complète.
- Comprendre le fonctionnement du protocole HTTP et ses limites en matière de sécurité.
- Configurer Apache : logs, droits d’accès aux dossiers, CGI, authentification, virtual hosts.
- Sécuriser les échanges avec HTTPS et une redirection permanente.
- Manipuler une base de données en SQL, la relier à PHP et gérer les droits des utilisateurs.

## Environnement

| Élément | Valeur |
|---|---|
| Serveur | Raspberry Pi — `clararaspberry` (192.168.0.206) |
| Client | PC Windows (192.168.0.100) |
| Logiciels | Apache 2.4.68, MariaDB 11.8.6, PHP 8.4.26, phpMyAdmin, WordPress |
| Outils | Wireshark, navigateur web, nano |

## Sommaire

| Partie | Contenu |
|---|---|
| [I. Intro et installation](Partie-I-intro-et-installation.md) | Présentation de LAMP, installation des paquets et démarrage des services Apache et MariaDB. |
| [II. Tests](Partie-II-tests.md) | Vérification du fonctionnement d’Apache, de la console SQL et de PHP (phpinfo). |
| [III. Utilisation](Partie-III-utilisation.md) | Installation de phpMyAdmin et déploiement de WordPress. |
| [IV. Apache](Partie-IV-apache.md) | Protocole HTTP et Wireshark, configuration d’Apache, logs, accès aux dossiers, CGI, protection des accès, serveurs virtuels et HTTPS. |
| [V. Utilisation de MySQL (MariaDB)](Partie-V-utilisation-de-mysql-mariadb.md) | Création d’une base, requêtes SQL, lien avec PHP, gestion des droits, sauvegarde et restauration. |

## Organisation du dépôt

```text
TP-LAMP/
├── README.md
├── Partie-I-intro-et-installation.md
├── Partie-II-tests.md
├── Partie-III-utilisation.md
├── Partie-IV-apache.md
├── Partie-V-utilisation-de-mysql-mariadb.md
└── captures/
```
