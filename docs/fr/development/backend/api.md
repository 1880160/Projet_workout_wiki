| Module  |  Contrôleur |  Service(s) | Référentiel/ ORM  |
|---|---|---|---|
|training.module   |UserExercise.Controller, Exercise.Controller   | UserExercise.service, Exercise.service |UserExercise, Exercise  |
| workout.module  | Workout.Controller  | Workout.service  |  Workout |   |
|  user.module | user.Controller  |  user.service | User  |
|   |   |   |   |   |

## Routes :

### Routes Workout

|Méthode|Route|Entrée (Body/Query/Params)|Description|
|--|--|--|--|
|GET|/workout| **Body** : {nom du workout / autres paramètres}| récupère tous les workouts, utilisé par les administrateurs
|GET|/workout/id|| récupère le workout par id, utilisé uniquement par l'administrateur |
|GET|/workout/my-workouts| **Query** : params : category=""&muscle_group=""&name=""| récupère les workouts de l'utilisateur |
|POST|/workout/create-workout| **Body** : un objet workout | Publie un nouveau workout sur le compte d'un utilisateur|
|DELETE|/workout/delete-workout| **Body** : un objet workout | Supprime un workout du compte d'un utilisateur|
|UPDATE|/workout/update-workout| **Body** : un objet workout | met à jour un workout du compte d'un utilisateur|

### Routes UserExercises

|Méthode|Route|Entrée (Body/Query/Params)|Description|
|--|--|--|--|
|GET|/user-exercise/| | récupère tous les exercices utilisateur, à utiliser uniquement par un administrateur|
|GET|/user-exercise/id| |récupère un exercice utilisateur par id, à utiliser uniquement par un administrateur |
|GET|/user-exercise/my-exercises|**Query** : récupère tous les exercices utilisateur|récupère un exercice utilisateur par id, à utiliser uniquement par un administrateur|
|UPDATE|/user-exercise/update-user-exercise|**Body** : un objet UserExercise | met à jour l'exercice d'un utilisateur|
|DELETE|/user-exercise/delete-user-exercise|**Body** : un objet UserExercise | supprime l'exercice d'un utilisateur|
|POST|/user-exercise/create-user-exercise|**Body** : un objet UserExercise | crée un UserExercise|

### Routes Exercise

|Méthode|Route|Entrée (Body/Query/Params)|Description|
|--|--|--|--|
|GET|/exercise/|  | récupère tous les exercices|
|GET|/exercise/id|  | récupère un exercice par id|
|POST|/exercise/create-exercise|**Body** : un objet Exercise| crée un exercice dans la base de données publique|
|UPDATE|/exercise/update-exercise|**Body** : un objet Exercise| met à jour un exercice dans la base de données publique|
|DELETE|/exercise/delete-exercise|**Body** : un objet Exercise| supprime un exercice dans la base de données publique|

### Routes des demandes d'exercice

|Méthode|Route|Entrée (Body/Query/Params)|Description|
|--|--|--|--|
|GET|/exercise-request/|  | récupérer tous les exercices|
|GET|/exercise-request/id|  | récupérer un exercice par id|
|POST|/exercise-request/create-exercise|**Body** : un objet Exercise| créer une demande d'exercice|
|UPDATE|/exercise-request/update-exercise|**Body** : un objet Exercise| mettre à jour une demande d'exercice |
|DELETE|/exercise-request/delete-exercise|**Body** : un objet Exercise| supprimer une demande d'exercice|

### Routes utilisateur

|Méthode|Route|Entrée (Body/Query/Params)|Description|
|--|--|--|--|
|POST|/user/sign-in|| se connecter à un compte|
|POST|/user/sign-up|| s'inscrire/créer un compte|
|GET| /user || récupérer tous les utilisateurs|
|GET| /user/id || récupérer un utilisateur par id|
|GET| /user/my-info || récupérer les informations de l'utilisateur actuel.|