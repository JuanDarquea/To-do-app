# ToDo List (Python CRUD App)

A simple command-line ToDo List application in Python that lets you manage your daily tasks. This project demonstrates basic CRUD (Create, Read, Update, Delete) functionality using file-based persistence (JSON), implemented in Spanish. 

**Features**
- Add Tasks: Create new to-do items with title, description, and optional deadline.
- List Tasks: View all your current tasks, their status, and deadlines.
- Modify Tasks: Edit the title, description, status (completed/pending), or deadline of existing tasks.
- Delete Tasks: Remove tasks from your list with confirmation to prevent accidents.
- Persistence: All tasks are saved to a tareas.json file, so your changes are not lost.
- Easy to Use: Simple command-line interface with clear prompts and error messages.

**File Structure**

├── ToDo-list.py       # Main program script

├── tareas.json        # Data file (auto-created on use)

└── README.md          # Project documentation

**Requirements**
- Python 3.7 or above (Standard Library only, uses json)

**Usage**
1. Download or clone this repository.
2. Open a terminal and run: python ToDo-list.py
3. Follow the on-screen menu instructions.


=== LISTA DE TAREAS ===
1. Agregar tarea
2. Ver todas las tareas
3. Modificar tarea
4. Eliminar tarea
5. Salir
=======================

**How Tasks Are Stored**
- Each task is saved in a JSON file with fields:
- id: Unique identifier
- titulo: Task title
- descripcion: Task description
- completada: Task status (True/False)
- fecha_creacion: Date created
- fecha_limite: Deadline (optional)

**Example:** json

{

  "id": 1,
  
  "titulo": "Estudiar Python",
  
  "descripcion": "Aprender CRUD básico",
  
  "completada": false,
  
  "fecha_creacion": "2025-01-15",
  
  "fecha_limite": "2025-01-20"
  
}


**Notes**
- The interface and prompts are in Spanish.
- If tareas.json does not exist, it will be created automatically.
- Handles user input errors gracefully.

**For Learners**

This project is ideal for those learning about:

- Python dictionaries and lists
- File I/O with JSON
- Structuring CLI programs
- Implementing CRUD operations
- Basic error and input handling

**Contribute**

Pull requests, ideas, and feedback are welcome to improve this simple project!


Enjoy managing your tasks and improving your Python skills!

Created by an aspiring data analyst and AI scientist for learning and demonstration purposes.
