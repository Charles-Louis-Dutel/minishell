# Minishell — École 42

Projet réalisé **en binôme**, développé en **C** dans le cadre du cursus de l'école 42.

L'objectif est de développer un interpréteur de commandes Unix reproduisant les principales fonctionnalités d'un shell comme Bash.

Ce projet permet d'approfondir la programmation système, la gestion des processus, la manipulation des descripteurs de fichiers et l'analyse de commandes.

## Fonctionnalités

- Affichage d'un prompt interactif et exécution de commandes.
- Analyse des commandes et de leurs arguments (parsing).
- Gestion des guillemets simples et doubles.
- Expansion des variables d'environnement (`$VAR`, `$?`).
- Recherche des exécutables à partir de la variable `PATH`.
- Exécution des commandes externes avec `fork()` et `execve()`.
- Gestion des pipes (`|`) et des redirections (`<`, `>`, `>>`, `<<`).
- Gestion des signaux (`Ctrl+C`, `Ctrl+D`, `Ctrl+\`).
- Implémentation des commandes internes : `echo`, `cd`, `pwd`, `export`, `unset`, `env` et `exit`.
- Gestion des codes de retour des commandes et des erreurs.

## Architecture

Le fonctionnement du shell repose sur plusieurs étapes :

1. **Lecture :** récupération de la commande saisie par l'utilisateur.
2. **Analyse :** identification des arguments, opérateurs et redirections.
3. **Expansion :** remplacement des variables d'environnement.
4. **Exécution :** lancement des commandes, gestion des pipes et des redirections.
5. **Nettoyage :** libération des ressources allouées.

## Compétences mises en œuvre

- Programmation en C
- Programmation système Unix/Linux
- Gestion des processus et des signaux
- Communication interprocessus
- Analyse syntaxique et traitement de chaînes
- Allocation dynamique et gestion de la mémoire
- Travail collaboratif et intégration de code

## Auteur

Charles-Louis Dutel — [GitHub](https://github.com/Charles-Louis-Dutel)

Projet réalisé en collaboration avec un autre étudiant de l'école 42.
