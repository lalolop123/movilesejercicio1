Lista de Tareas — Android (Kotlin + Jetpack Compose)

Aplicación de lista de tareas ("To-Do List") desarrollada como proyecto práctico, que permite agregar, completar y eliminar tareas.

Funcionalidades
Agregar nuevas tareas mediante un campo de texto.
Visualizar la lista de tareas en tiempo real.
Marcar tareas como completadas (se muestran tachadas y en gris).
Eliminar tareas deslizando la fila hacia la izquierda.
Tecnologías utilizadas
Kotlin
Jetpack Compose (UI declarativa)
Material 3
Estado en memoria (remember, mutableStateListOf) — sin persistencia entre sesiones.
Arquitectura
Task: data class que representa una tarea (id, título, estado de completado).
TaskListScreen: pantalla principal, contiene el estado de la lista y la lógica de agregar/eliminar.
TaskRow: componente stateless (sin estado propio) que recibe los datos de la tarea y comunica eventos hacia el componente padre mediante lambdas (patrón de state hoisting).

Requisitos mínimos
Android Studio actualizado.
minSdk 24.

Nota
Este proyecto no incluye persistencia de datos (Room, DataStore) por estar fuera del alcance de la tarea original; las tareas se pierden al cerrar la app. Queda como posible mejora futura.
