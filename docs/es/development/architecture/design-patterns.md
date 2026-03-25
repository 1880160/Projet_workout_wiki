# Patrones de diseño utilizados en el proyecto

## Composite

El patrón composite se utilizará para estructurar nuestras rutas. Por lo tanto, las subrutas estarán contenidas dentro de subcarpetas en una estructura similar a las rutas del api/frontend.

## Singleton

NestJs utiliza singleton por defecto en su repositorio.

## Decorator

Se utilizará Decorator para inyectar código dentro de funciones y rutas
para reducir considerablemente la cantidad de código y aumentar la legibilidad del código.

## Observer

El servidor utilizará SSE (Server Side Events) para notificar al cliente sobre notificaciones en tiempo real, como alertas de entrenamiento y solicitudes de revisión de ejercicios.
