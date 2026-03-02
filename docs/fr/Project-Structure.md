# Structure du projet

## Backend

### Structure du système backend

![texte alternatif](./../Diagrams/ImageRenditions/SystemDiagram.png)

| Module  |  Contrôleur |  Service(s) | Repository/ ORM  |
|---|---|---|---|
|training.module   |UserProgress.Controller, Exercise.Controller   | UserProgress.service, Exercise.service |UserProgress, Exercise  |
| workout.module  | Workout.Controller  | Workout.service  |  Workout |   |
|  user.module | user.Controller  |  user.service | User  |
|   |   |   |   |   |

## Routes :

|Méthode|Route|Entrée (Body/Query/Params)|Description|
|--|--|--|--|
|GET|/workout| **Body** : {nom de l'entraînement (nommé par l'utilisateur)}|z|
|POST|/workout| **Body** : {liste des entraînements}|z|
|Inputs|/workout|  |z|
|POST|/excerice|nom de l'exercice, muscle ciblé, , |y|
|POST|/userprogress|répétition/temps, série, poids|y|
|POST|/user|nom|y|

### /Workout

### Get

Retourne les « Workouts » associés à l'utilisateur

#### Entrées

- jeton de connexion

#### Sortie

les entraînements associés à l'utilisateur

### Post

Crée un nouvel entraînement associé à l'utilisateur

#### Entrées

- l'utilisateur connecté
- l'objet User : (nom, mot de passe, etc.)

#### Sortie

Retourne la réponse à l'action

### Put/Patch

modifie un entraînement dont l'ID est x et qui est associé à l'utilisateur.

#### Entrées

- l'utilisateur connecté
- l'ID de l'utilisateur à modifier
- les attributs à modifier

#### Sortie

Retourne la réponse à l'action

## /UserProgress (Mon exercice)

### Get

Retourne le "UserProgress" associé à l'utilisateur

#### Entrée

- l'utilisateur connecté

#### Sortie

Liste des "UserProgress" associés à l'utilisateur

### Post

Crée un nouveau "UserProgress" associé à l'utilisateur

#### Entrée

- L'utilisateur connecté
- L'objet "UserProgress" à créer

#### Sortie

Retourne la réponse à l'action

### Put/Patch

Modifie un "UserProgress" dont l'ID est associé à l'utilisateur.

#### Entrée

- L'utilisateur connecté
- L'ID UserProgress
- L'objet UserProgress à modifier

#### Sortie

Retourne la réponse à l'action

## /Exercise

### Get

Retourne les exercices

#### Entrée

- (Optionnel) "Query" pour le filtrage

#### Sortie

Liste des exercices filtrés

### Post

Soumettre une demande de création pour validation

#### Entrée

- ID de l'utilisateur créant l'exercice
- Objet de l'exercice à créer

#### Sortie

Retourne la réponse à l'action
