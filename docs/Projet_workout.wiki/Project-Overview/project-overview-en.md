## A clear description of the application

The software allows you to create a server that manages user data for a training application. It enables synchronization of workouts across multiple user interfaces available on several platforms. This application will allow users to easily track their progress, know which exercise to do according to their needs and how to perform it correctly, and get inspired.

## The problem statement and objectives (framework)

This application solves the problem of synchronizing workouts across multiple platforms in a user interface designed for training.

The objective is to create a self-hosted and open-source application that is simple, documented, and exclusively for workouts.

## An overview of the application's features

- Create custom workouts (the user will be able to select exercises and then create workouts which are lists of exercises)
- Progress tracking (the user will enter the number of reps/time, sets, and weight).
- Exercise search with or without filtering

## Description of users and roles

### Developers

Other users who wish to participate in improving the application.

### Users

Users who wish to host the application.

## Functional and non-functional requirements

### Functional

- Database: user, exercises, list of exercises created by user, workout.
- REST API
- Creation of a training session
- Exercise searches
- Progress tracking
- Administrative validation

### Non-functional

- SOLID principles
- Clear documentation

## Application constraints

- Backend: Next.js
- Frontend: Angular

## Use cases

<img width="526" height="788" alt="livrable_use_case drawio" src="https://github.com/user-attachments/assets/9eaeb3dd-3473-4b00-815a-f287c2709ef4" />

### Use case specifications:

#### Search for an exercise:

| Description  |  Search the public database for an exercise |
|---|---|
|  Actors |  User |

#### Add an exercise:

| Description  | Add an exercise to the public database |
|---|---|
|  Actors | User |

#### Add user progress to an exercise:

| Description  | Add user progress linked to the user, specifying weight, duration, etc. |
|---|---|
|  Actors | User |

#### Modify user progress for an exercise:

| Description  | Modify user progress linked to the user, specifying weight, duration, etc. |
|---|---|
|  Actors | User |

#### Create a workout:

| Description  | Create a workout linked to a user |
|---|---|
|  Actors | User |

#### Modify a workout:

| Description  | Modify a workout linked to a user |
|---|---|
|  Actors | User |

## Planning through the development methodology

Planning will take place weekly during the course period, ensuring that objectives are met. Additionally, the development methodology will be iterative, allowing for project reorganization in case of issues.
The project will be divided into three trimesters:
- Initial API development
- Frontend
- Deployment
