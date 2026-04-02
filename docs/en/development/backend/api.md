| Module  |  Controller |  Service(s) | Repository/ ORM  |
|---|---|---|---|
|exercise.module   |UserExercise.Controller, Exercise.Controller   | UserExercise.service, Exercise.service |UserExercise, Exercise  |
| workout.module  | Workout.Controller  | Workout.service  |  Workout |   |
|  user.module | user.Controller  |  user.service | User  |
|   |   |   |   |   |

## Routes:

### Workout routes
|Method|Route|Input(Body/Query/Params)|Description|
|--|--|--|--|
|GET|/workout| **Body**: {workout name/ other parameters}| get all workout, used by admins
|GET|/workout/id|| get the workout by id, only used by admin |
|GET|/workout/my-workouts| **Query** : params : category=""&muscle_group=""&name=""| get the users' workout |
|POST|/workout/create-workout| **Body**: a workout object | Post a new workout to a user's account|
|DELETE|/workout/delete-workout| **Body**: a workout object | Deleta a workout from a user's account|
|UPDATE|/workout/update-workout| **Body**: a workout object | update a workout from a user's account|

### UserExercises routes
|Method|Route|Input(Body/Query/Params)|Description|
|--|--|--|--|
|GET|/user-exercise/| | get all User exercise, only to be used by an admin|
|GET|/user-exercise/id| |get an user exercise by id, only to be used by an admin |
|GET|/user-exercise/my-exercises|**Query**: get all user exercise|get an user exercise by id, only to be used by an admin|
|UPDATE|/user-exercise/update-user-exercise|**Body**: a UserExercise object | update's a user's exercise|
|DELETE|/user-exercise/delete-user-exercise|**Body**: a UserExercise object | delete a user's exercise|
|POST|/user-exercise/create-user-exercise|**Body**: a UserExercise object | create a UserExercise|

### Exercise routes
|Method|Route|Input(Body/Query/Params)|Description|
|--|--|--|--|
|GET|/exercise/|  | get all exercise|
|GET|/exercise/id|  | get an exercise by id|
|POST|/exercise/create-exercise|**Body**: a Exercise object| create a  exercise in the public database|
|UPDATE|/exercise/update-exercise|**Body**: a Exercise object| update a exercise in the public database|
|DELETE|/exercise/delete-exercise|**Body**: a Exercise object| delete a  exercise in the public database|


### Exercise Request routes
|Method|Route|Input(Body/Query/Params)|Description|
|--|--|--|--|
|GET|/exercise-request/|  | get all exercise|
|GET|/exercise-request/id|  | get an exercise by id|
|POST|/exercise-request/create-exercise|**Body**: a Exercise object| create a exercise requeste|
|UPDATE|/exercise-request/update-exercise|**Body**: a Exercise object| update a exercise request |
|DELETE|/exercise-request/delete-exercise|**Body**: a Exercise object| delete a exercise request|


### User routes
|Method|Route|Input(Body/Query/Params)|Description|
|--|--|--|--|
|POST|/user/sign-in|| sign in into an account|
|POST|/user/sign-up|| sign up/creates an account|
|GET| /user || gets all the users|
|GET| /user/id || gets all the users|
|GET| /user/my-info || gets the current user's info.|