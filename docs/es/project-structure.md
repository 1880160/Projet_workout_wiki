# Estructura del proyecto

## Backend

### Estructura del sistema backend

![texto alternativo](./../Diagrams/ImageRenditions/SystemDiagram.png)

| Módulo  |  Controlador |  Servicio(s) | Repositorio/ ORM  |
|---|---|---|---|
|training.module   |UserProgress.Controller, Exercise.Controller   | UserProgress.service, Exercise.service |UserProgress, Exercise  |
| workout.module  | Workout.Controller  | Workout.service  |  Workout |   |
|  user.module | user.Controller  |  user.service | User  |
|   |   |   |   |   |

## Rutas:

|Método|Ruta|Entrada(Body/Query/Params)|Descripción|
|--|--|--|--|
|GET|/workout| **Body**: {nombre del entrenamiento (nombrado por el usuario)}|z|
|POST|/workout| **Body**: {lista de entrenamientos}|z|
|Inputs|/workout|  |z|
|POST|/excerice|nombre del ejercicio, músculo objetivo, , |y|
|POST|/userprogress|repetición/tiempo, serie, peso|y|
|POST|/user|nombre|y|

### /Workout

### Get

Devuelve los "Entrenamientos" asociados con el usuario

#### Entradas

- token de inicio de sesión

#### Salida

los entrenamientos asociados con el usuario

### Post

Crea un nuevo entrenamiento asociado con el usuario

#### Entradas

- el usuario con sesión iniciada
- el objeto User: (nombre, contraseña, etc.)

#### Salida

Devuelve la respuesta a la acción

### Put/Patch

modifica un entrenamiento cuyo ID es x y que está asociado con el usuario.

#### Entradas

- el usuario con sesión iniciada
- el ID del usuario a modificar
- los atributos a modificar

#### Salida

Devuelve la respuesta a la acción

## /UserProgress (Mi ejercicio)

### Get

Devuelve el "UserProgress" asociado con el usuario

#### Input

- el usuario autenticado

#### Output

Lista de "UserProgress" asociados con el usuario

### Post

Crea un nuevo "UserProgress" asociado con el usuario

#### Input

- El usuario autenticado
- El objeto "UserProgress" a crear

#### Output

Devuelve la respuesta a la acción

### Put/Patch

Modifica un "UserProgress" cuyo ID está asociado con el usuario.

#### Input

- El usuario autenticado
- El ID de UserProgress
- El objeto UserProgress a modificar

#### Output

Devuelve la respuesta a la acción

## /Exercise

### Get

Devuelve los ejercicios

#### Input

- (Opcional) "Query" para filtrar

#### Salida

Lista de ejercicios filtrados

### Post

Enviar una solicitud de creación para validación

#### Entrada

- ID del usuario que crea el ejercicio
- Objeto del ejercicio a crear

#### Salida

Devuelve la respuesta a la acción
