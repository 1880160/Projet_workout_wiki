## Una descripción clara de la aplicación

El software te permite crear un servidor que gestiona los datos de usuario para una aplicación de entrenamiento. Permite la sincronización de entrenamientos a través de múltiples interfaces de usuario disponibles en varias plataformas. Esta aplicación permitirá a los usuarios hacer seguimiento fácilmente de su progreso, saber qué ejercicio hacer según sus necesidades y cómo realizarlo correctamente, y obtener inspiración.

## El planteamiento del problema y objetivos (marco)

Esta aplicación resuelve el problema de sincronizar entrenamientos a través de múltiples plataformas en una interfaz de usuario diseñada para entrenamiento.

El objetivo es crear una aplicación auto-alojada y de código abierto que sea simple, documentada y exclusivamente para entrenamientos.

## Una visión general de las funcionalidades de la aplicación

- Crear entrenamientos personalizados (el usuario podrá seleccionar ejercicios y luego crear entrenamientos que son listas de ejercicios)
- Seguimiento de progreso (el usuario introducirá el número de repeticiones/tiempo, series y peso).
- Búsqueda de ejercicios con o sin filtros

## Descripción de usuarios y roles

### Desarrolladores

Otros usuarios que deseen participar en mejorar la aplicación.

### Usuarios

Usuarios que deseen alojar la aplicación.

## Requisitos funcionales y no funcionales

### Funcionales

- Base de datos: usuario, ejercicios, lista de ejercicios creados por usuario, entrenamiento.
- API REST
- Creación de una sesión de entrenamiento
- Búsquedas de ejercicios
- Seguimiento de progreso
- Validación administrativa

### No funcionales

- Principios SOLID
- Documentación clara

## Restricciones de la aplicación

- Backend: Next.js
- Frontend: Angular

## Casos de uso

<img width="526" height="788" alt="livrable_use_case drawio" src="https://github.com/user-attachments/assets/9eaeb3dd-3473-4b00-815a-f287c2709ef4" />

### Especificaciones de casos de uso:

#### Buscar un ejercicio:

| Descripción  |  Buscar un ejercicio en la base de datos pública |
|---|---|
|  Actores |  Usuario |

#### Añadir un ejercicio:

| Descripción  | Añadir un ejercicio a la base de datos pública |
|---|---|
|  Actores | Usuario |

#### Añadir progreso del usuario a un ejercicio:

| Descripción  | Añadir progreso del usuario vinculado al usuario, especificando peso, duración, etc. |
|---|---|
|  Actores | Usuario |

#### Modificar progreso del usuario para un ejercicio:

| Descripción  | Modificar progreso del usuario vinculado al usuario, especificando peso, duración, etc. |
|---|---|
|  Actores | Usuario |

#### Crear un entrenamiento:

| Descripción  | Crear un entrenamiento vinculado a un usuario |
|---|---|
|  Actores | Usuario |

#### Modificar un entrenamiento:

| Descripción  | Modificar un entrenamiento vinculado a un usuario |
|---|---|
|  Actores | Usuario |

## Planificación a través de la metodología de desarrollo

La planificación se llevará a cabo semanalmente durante el período del curso, asegurando que se cumplan los objetivos. Además, la metodología de desarrollo será iterativa, permitiendo la reorganización del proyecto en caso de problemas.
El proyecto se dividirá en tres trimestres:
- Desarrollo inicial de la API
- Frontend
- Despliegue
