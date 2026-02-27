## Backend

- [  ] 3 modules
- [  ]

### Backend system structure

![alt text](./../Diagrams/ImageRenditions/SystemDiagram.png)

| Module  |  Controller |  Service(s) | Repository/ ORM  |
|---|---|---|---|
|training.module   |Workout.Controller, UserProgress.Controller, Exercise.Controller   |  Workout.service, UserProgress.service, Exercise.service | Workout, UserProgress, Exercise  |
|  user.module | user.Controller  |  user.service | User  |
|   |   |   |   |   |

## Routes:

|Method|Route|Input(Body/Query/Params)|Description|
|--|--|--|--|
|GET|/workout| **Body**: {workout name(named by the user)}|z|
|POST|/workout| **Body**: {list of training}|z|
|Inputs|/workout|  |z|
|POST|/excerice|exercise name, targeted muscle, , |y|
|POST|/userprogress|repetition/time, set, weight|y|
|POST|/user|name|y|

### /Workout

### Get

Returns the "Workouts" associated with the user

#### Inputs

- login token

#### Output

the workouts associated with the user

### Post

Creates a new workout associated with the user

#### Inputs

- the logged-in user
- the User object: (Name, Password, etc.)

#### Output

Returns the response to the action

### Put/Patch

modifies a workout whose ID is x and which is associated with the user.

#### Inputs

- the logged-in user
- the ID of the user to modify
- the attributes to modify

#### Output

Returns the response to the action

## /UserProgress (My Exercise)

### Get

Returns the "UserProgress" associated with the user

#### Input

- the logged-in user

#### Output

List of "UserProgress" associated with the user

### Post

Creates a new "UserProgress" associated with the user

#### Input

- The logged-in user
- The "UserProgress" object to create

#### Output

Returns the response to the action

### Put/Patch

Modifies a "UserProgress" whose ID is associated with the user.

#### Input

- The logged-in user
- The UserProgress ID
- The UserProgress object to modify

#### Output

Returns the response to the action

## /Exercise

### Get

Returns the exercises

#### Input

- (Optional) "Query" for filtering

#### Output

List of filtered exercises

### Post

Submit a creation request for validation

#### Input

- ID of the user creating the exercise
- Object of the exercise to be created

#### Output

Returns the response to the action
