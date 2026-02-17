# ToDo List (Aplicación CRUD en python)

Una aplicación sencilla de lista de tareas para la línea de comandos desarrollada en Python. Este proyecto demuestra las funcionalidades básicas de un sistema CRUD (Crear, Leer, Actualizar, Borrar) utilizando persistencia de datos en archivos JSON.

## Características
- Agregar Tareas: Crea nuevos elementos con título, descripción y fecha límite opcional.
- Listar Tareas: Visualiza todas tus tareas actuales, su estado y sus plazos.
- Modificar Tareas: Edita el título, la descripción, el estado (completada/pendiente) o la fecha límite.
- Eliminar Tareas: Quita tareas de la lista con una confirmación previa para evitar accidentes.
- Persistencia: Todos los cambios se guardan en un archivo tareas.json, por lo que la información no se pierde al cerrar el programa.
- Fácil de usar: Interfaz de línea de comandos (CLI) intuitiva con mensajes claros y manejo de errores.

## Estructura del Proyecto
```
To-do-list
|
├── ToDo-list.py       # Script principal del programa
├── tareas.json        # Archivo de datos (se crea automáticamente)
└── README.md          # Documentación del proyecto
```

## Requisitos
- Python 3.7 o superior.
- Solo utiliza la Librería Estándar de Python (módulo json).

## Uso
1. Descarga o clona este repositorio.
2. Abre una terminal y ejecuta:

    `python ToDo-list.py`

3. Sigue las instrucciones del menú en pantalla:

```
=== LISTA DE TAREAS ===
1. Agregar tarea
2. Ver todas las tareas
3. Modificar tarea
4. Eliminar tarea
5. Salir
=======================
```

## Almacenamiento de Datos
Cada tarea se guarda en el archivo JSON con los siguientes campos:

- id: Identificador único.
- titulo: Nombre de la tarea.
- descripcion: Detalle de la tarea.
- completada: Estado de la tarea (True/False).
- fecha_creacion: Fecha en que se registró.
- fecha_limite: Plazo de entrega (opcional).

**Ejemplo de formato JSON:** 
```
json

{
  "id": 1,  
  "titulo": "Estudiar Python",  
  "descripcion": "Aprender CRUD básico",  
  "completada": false,  
  "fecha_creacion": "2025-01-15",  
  "fecha_limite": "2025-01-20"  
}
```

## Notas Adicionales
- Tanto la interfaz como los mensajes de usuario están en español.
- Si el archivo `tareas.json` no existe, el sistema lo generará automáticamente al guardar la primera tarea.
- El programa gestiona errores de entrada (como ingresar letras en campos numéricos) de manera controlada.

## Ideal para Estudiantes
Este proyecto es perfecto para quienes están aprendiendo sobre:

1. Diccionarios y listas en Python.
2. Entrada y salida de archivos (File I/O) con JSON.
3. Estructuración de programas CLI.
4. Lógica de operaciones CRUD.
5. Manejo básico de errores y excepciones.

## Contribuciones
¡Cualquier pull request, idea o sugerencia es bienvenida para mejorar este proyecto!

¡Espero que disfrutes gestionando tus tareas mientras sigues puliendo tus habilidades en Python!

Creado por un aspirante a Analista de Datos y Científico de IA con fines de aprendizaje y demostración.
