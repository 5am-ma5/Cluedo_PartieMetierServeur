PSD4S – Cluedo Client/Serveur
Description

Ce projet a été réalisé dans le cadre du module PSD4S. Il consiste en l'implémentation d'une version réseau du jeu Cluedo reposant sur une architecture client/serveur.

Le serveur est responsable de la gestion complète des règles du jeu, des joueurs connectés, du plateau, de la distribution des cartes et du déroulement des parties. Les communications entre les clients et le serveur sont effectuées au moyen d'un protocole textuel défini dans l'énoncé du projet.

Fonctionnalités implémentées
Connexion et déconnexion des joueurs.
Démarrage d'une partie.
Distribution automatique des cartes.
Gestion des déplacements sur le plateau.
Gestion des passages secrets.
Lancer de dés.
Émission et réfutation des soupçons.
Gestion des accusations.
Détermination du vainqueur.
Gestion des erreurs liées aux règles du jeu.
Tests d'intégration des principales fonctionnalités.
Structure du projet
Métier
Superviseur.java : gestion globale de la partie.
Joueur.java : représentation d'un joueur.
Hypothese.java : représentation d'un soupçon ou d'une accusation.
PlateauCluedo.java : gestion du plateau de jeu.
CaseCluedo.java : représentation d'une case du plateau.
Carte.java : classe de base des cartes.
EPersonnage.java, EArme.java, ELieu.java : énumérations des cartes.
Réseau
Serveur.java : serveur principal.
ConnexionUtilisateur.java : gestion des connexions.
ThreadConnexion.java : communication avec les clients.
ThreadAcceptConnexion.java : acceptation des nouvelles connexions.
Experts

Les classes Expert* implémentent l'interprétation des différentes commandes du protocole :

Connexion
Déconnexion
Démarrage de partie
Déplacement
Lancer de dés
Soupçon
Réfutation
Accusation
Fin de tour
Messagerie
Tests

Les tests d'intégration sont regroupés dans :

src/reseau/integration/Tests

Ils permettent de vérifier le bon fonctionnement des principales fonctionnalités du serveur.

Compilation et exécution

Le point d'entrée de l'application est :

src/main/Main.java

Le projet est développé en Java et nécessite un JDK compatible avec la version utilisée lors du développement.

Auteurs

Projet réalisé dans le cadre du module PSD4S – Université de Lorraine.
