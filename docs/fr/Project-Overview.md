## Une description claire de l’application

Le logiciel permet de créer un serveur qui gère les données des utilisateurs pour une application d’entrainement. Permettant de synchroniser les entrainements à travers plusieurs interfaces utilisateur disponibles sur plusieurs plateformes. Cette application permettra aux utilisateurs de facilement suivrent leur progression, de savoir quel exercice à faire selon leur besoin et comment bien l'exécuter et de s'inspirer.

## La problématique et les objectifs (cadre)

Cette application résout la problématique de synchronisation des entrainements à travers plusieurs plates-formes dans une interface utilisateur ciblée pour l'entrainement. 

L'objectif est de créer une application «self-hosted» et «Open-Source» qui est simple, documenté et uniquement pour les entrainements.

## Une vue d’ensemble des fonctions de l’application

- Créer des entrainements personnalisés (l'utilisateur pourra sélectionner des exercices et pourra ensuite créer des entrainements qui sont des listes d'exercices )
- Suivi de la progression ( l'usager entrera le nombre de reps/temps, de «sets» et le poids).
- Recherche d'exercice avec ou sans filtrage

## La description des utilisateurs et des rôles

### Developeurs

D'autres utilisateurs qui désirent participer à l'amélioration de l'application.

### Utilisateurs

Les utilisateurs qui désirent héberger l'application.

## Les exigences fonctionnelles et non fonctionnelles

### Fonctionnelles

- Base de données : utilisateur, exercices, liste d'exercices crée par utilisateur, entrainement.
- API Rest
- Création d'une scéance d'entrainement
- Recherches d'exercices
- Suivi de progression
- Validation Administrative

### non fonctionnelles

- Principe SOLID
- Documentation claire

## Les contraintes de l'application ;

- backend: Nextjs
- frontend : Angular

## Les cas d’utilisation (use cases) ;

![Use case diagram](../Diagrams/ImageRenditions/livrable_use_case.png)

### Spécifications des cas d'utilisation:

#### Chercher un exercise:

| Description  |  Chercher la base de données publique  pour un exercice |
|---|---|
|  Acteurs |  Utilisateur |

#### Ajouter un exercise:

| Description  | Ajouter un exercice dans la base de données publique |
|---|---|
|  Acteurs | Utilisateur |

#### Ajouter un progres Utilisateur a un exercise:

| Description  | Ajouter un Progrès utilisateur relié à l'utilisateur, spécifie le poids, la dure et, etc. |
|---|---|
|  Acteurs | Utilisateur |

#### Modifier un progres Utilisateur a un exercise:

| Description  | Modifie un Progres Utilisateur relié à l'utilisateur, spécifie le poids, la dure et, etc. |
|---|---|
|  Acteurs | Utilisateur |

#### Creer un entrainement:

| Description  | Créer un entrainement relié à un utilisateur |
|---|---|
|  Acteurs | Utilisateur |

#### Modifier un entrainement:

| Description  | Modifie un entrainement relié à un utilisateur |
|---|---|
|  Acteurs | Utilisateur |

## La planification à travers la méthodologie de développement ;

La planification sera chaque semaine durant la période de cours. S'assurant que les objectifs seront atteints. Aussi, la méthodologie de développement sera itérative, permettant de réorganiser le projet dans le cas où il y a des problèmes.
Le projet sera séparé en trois Trieste:
- Development Initiale API
- Frontend 
- Deployment
