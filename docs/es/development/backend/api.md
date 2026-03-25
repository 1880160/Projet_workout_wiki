| Módulo  |  Controlador |  Servicio(s) | Repositorio/ ORM  |
|---|---|---|---|
|training.module   |UserExercise.Controller, Exercise.Controller   | UserExercise.service, Exercise.service |UserExercise, Exercise  |
| workout.module  | Workout.Controller  | Workout.service  |  Workout |   |
|  user.module | user.Controller  |  user.service | User  |
|   |   |   |   |   |

## Rutas:

### Rutas de entrenamiento

|Método|Ruta|Entrada(Body/Query/Params)|Descripción|
|--|--|--|--|
|GET|/workout| **Body**: {nombre del entrenamiento/ otros parámetros}| obtener todos los entrenamientos, usado por administradores
|GET|/workout/id|| obtener el entrenamiento por id, solo usado por administrador |
|GET|/workout/my-workouts| **Query** : params : category=""&muscle_group=""&name=""| obtener los entrenamientos del usuario |
|POST|/workout/create-workout| **Body**: un objeto workout | Publicar un nuevo entrenamiento en la cuenta de un usuario|
|DELETE|/workout/delete-workout| **Body**: un objeto workout | Eliminar un entrenamiento de la cuenta de un usuario|
|UPDATE|/workout/update-workout| **Body**: un objeto workout | actualizar un entrenamiento de la cuenta de un usuario|

### Rutas de ejercicios de usuario

|Método|Ruta|Entrada(Body/Query/Params)|Descripción|
|--|--|--|--|
|GET|/user-exercise/| | obtener todos los ejercicios de usuario, solo para ser usado por un administrador|
|GET|/user-exercise/id| |obtener un ejercicio de usuario por id, solo para ser usado por un administrador |
|GET|/user-exercise/my-exercises|**Query**: obtener todos los ejercicios de usuario|obtener un ejercicio de usuario por id, solo para ser usado por un administrador|
|UPDATE|/user-exercise/update-user-exercise|**Body**: un objeto UserExercise | actualizar el ejercicio de un usuario|
|DELETE|/user-exercise/delete-user-exercise|**Body**: un objeto UserExercise | eliminar el ejercicio de un usuario|
|POST|/user-exercise/create-user-exercise|**Body**: un objeto UserExercise | crear un UserExercise|

### Rutas de ejercicios

|Método|Ruta|Entrada(Body/Query/Params)|Descripción|
|--|--|--|--|
|GET|/exercise/|  | obtener todos los ejercicios|
|GET|/exercise/id|  | obtener un ejercicio por id|
|POST|/exercise/create-exercise|**Body**: un objeto Exercise| crear un ejercicio en la base de datos pública|
|UPDATE|/exercise/update-exercise|**Body**: un objeto Exercise| actualizar un ejercicio en la base de datos pública|
|DELETE|/exercise/delete-exercise|**Body**: un objeto Exercise| eliminar un ejercicio en la base de datos pública|

### Rutas de Solicitud de Ejercicio

|Método|Ruta|Entrada(Body/Query/Params)|Descripción|
|--|--|--|--|
|GET|/exercise-request/|  | obtener todos los ejercicios|
|GET|/exercise-request/id|  | obtener un ejercicio por id|
|POST|/exercise-request/create-exercise|**Body**: un objeto Exercise| crear una solicitud de ejercicio|
|UPDATE|/exercise-request/update-exercise|**Body**: un objeto Exercise| actualizar una solicitud de ejercicio|
|DELETE|/exercise-request/delete-exercise|**Body**: un objeto Exercise| eliminar una solicitud de ejercicio|

### Rutas de Usuario

|Método|Ruta|Entrada(Body/Query/Params)|Descripción|
|--|--|--|--|
|POST|/user/sign-in|| iniciar sesión en una cuenta|
|POST|/user/sign-up|| registrarse/crear una cuenta|
|GET| /user || obtener todos los usuarios|
|GET| /user/id || obtener un usuario por id|
|GET| /user/my-info || obtener la información del usuario actual|