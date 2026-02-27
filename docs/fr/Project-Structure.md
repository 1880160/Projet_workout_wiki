## Backend

- [  ] 3 modules
- [  ]

### Structure de système backend

![alt text](./../Diagrams/ImageRenditions/SystemDiagram.png)

| Module  |  Controller |  Service(s) | Repository/ ORM  |
|---|---|---|---|
|training.module   |Workout.Controller, UserProgress.Controller, Exercise.Controller   |  Workout.service, UserProgress.service, Exercise.service | Workout, UserProgress, Exercise  |
|  user.module | user.Controller  |  user.service | User  |
|   |   |   |   |   |

## Routes:

|Methode|Route|Entre(Body/Query/Params)|Description|
|--|--|--|--|
|GET|/workout| **Body**: {nom du workout(named by the user)}|z|
|POST|/workout| **Body**: {list of training}|z|
|Inputs|/workout|  |z|
|POST|/excerice|nom exercise, muscle sollicité, , |y|
|POST|/userprogress|repetition/temps, série, poids|y|
|POST|/user|nom|y|

### /Workout

### Get

Retourne les «Workout» associés à l'utilisateur

#### Inputs

- token de connexion

#### Output

les Workouts associer à l'utilisateur

### Post

Crée un nouveau Workout associer à l'utilisateur

#### Inputs

- l'utilisateur connectée
- l'objet User : (Nom, Mot de passe et ect...)

#### Output

Retourne la réponse à l'action

### Put/Patch

modifie un Workout dont l'ID est x et qui est associer à l'utilisateur.

#### Inputs

- l'utilisateur connectée
- l'Id de l'user à modifier
- les attributs à modifier

#### Output

Retourne la réponse à l'action

## /UserProgress (My Exercise)

### Get

Retourne les «UserProgress» associer à l'utilisateur

#### Input

- l'utilisateur connecté

#### Output

List des «UserProgres» associer à l'utilisateur

### Post

Crée un nouveau «UserProgress» associer à l'utilisateur

#### Input

- L'utilisateur connecté
- L'objet «UserProgress» à cree

#### Output

Retourne la réponse à l'action

### Put/Patch

Modifie un «UserProgress» dont le ID est associé à l'utilisateur.

#### Input

- L'utilisateur connecté
- L'ID du UserProgress
- L'objet UserProgress à modifier

#### Output

Retourne la réponse à l'action

## /Exercise

### Get

Retourne les exercises

#### Input

- (Optional) «Query» pour le filtrage

#### Output

List des exercises filtrers

### Post

Émets une requête de création pour validation

#### Input

- ID de l'utilisateur qui crée l'exercice
- Objet de l'exercise à crée

#### Output

Retourne la réponse à l'action

## Composite

Le pattern composite sera utilisé pour structurer nos routes. Par conséquent, les sous-routes seront contenues dans des sous-dossiers dans une structure similaire aux routes de l'api/frontend.

## Singleton

NestJs utilise le singleton par défaut dans son repository.

## Decorator

Le decorator sera utilisé pour injecter du code dans les fonctions et les routes
afin de réduire considérablement la quantité de code et d'améliorer la lisibilité du code.
