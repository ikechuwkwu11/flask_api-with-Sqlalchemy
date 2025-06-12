# 📝 Flask To-Do REST API
A simple RESTful API built using Flask, Flask-RESTful, and SQLAlchemy that allows users to perform CRUD operations on a list of to-do tasks.

## 🔧 Features
- Create a new to-do task
- View a single task by ID or all tasks
- Update a task (partial updates supported)
- Delete a task
- Uses SQLite for lightweight database support
- Includes basic error handling with helpful messages

## 🧰 Tech Stack
- Technology	Purpose
- Python 3.x	Programming language
- Flask	Web framework
- Flask-RESTful	Building RESTful APIs
- SQLAlchemy	ORM for interacting with the database
- SQLite	Default database (file-based)

## 📄 Get All To-Dos
- GET /todos
- Returns a dictionary of all tasks by ID.

## 📄 Get a Specific To-Do
- GET /todos/<todo_id>

## ❌ Delete a To-Do
- DELETE /todos/<todo_id>

## ⚠️ Error Handling
- 404 – Task not found
- 409 – Task ID already exists or can't update/delete a nonexistent task

## 📌 Notes
- Database is initialized using db.create_all() on app start.
- Uses marshal_with for serializing responses from SQLAlchemy models.
- Add requirements.txt by running:
