# Funcionalidades

Aquí está la lista de funcionalidades que están planificadas o en debate.

## Funcionalidades planificadas

Estas son las funcionalidades en las que se enfocará el desarrollo, ya que están confirmadas como necesarias o deseadas para la aplicación.
Ten en cuenta que las correcciones de errores y la refactorización del código de la aplicación no están incluidas aquí.

### La página de "Reproducir/Ejecutar" entrenamiento

Esta página está diseñada para ser utilizada durante un entrenamiento. Tendrá una interfaz simple que mostrará los ejercicios de una sesión de entrenamiento. Incluirá funcionalidades como un temporizador, una forma de marcar los ejercicios como completados y cambio automático de ejercicios para entrenamientos tipo circuito.

### Aplicación móvil con capacitorjs

El frontend recibirá una versión móvil utilizando Capacitor. Esto facilitará el uso de la aplicación cuando se utilice lejos de un ordenador. Además, Capacitor no requiere reescribir la implementación web, por lo que será fácil sincronizarla con la interfaz web.

## Funcionalidades en debate

Estas son funcionalidades que aún no están confirmadas, pero se están considerando seriamente.

### Hacer que la aplicación priorice el cliente

Esto permitirá que la aplicación no requiera un backend para funcionar. Solo necesitará el backend para sincronizar.
Podrían utilizarse RxDB, Powersync o Electric SQL para sincronizar una base de datos SQLite local con una base de datos más grande.
