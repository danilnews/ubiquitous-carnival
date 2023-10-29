
Simple To-Do List Web Application

Overview

This is a simple web application that allows users to manage a list of tasks. Users can add, edit, delete tasks, and view the history of their changes.

Project Structure


Backend (Go)
Directory Structure:
- main.go: Main file to run our server.
- handlers/: Folder containing HTTP request handlers.
  - tasks.go: Handlers for managing tasks (add, edit, delete, list).
- models/: Folder for data models.
  - task.go: Data model for tasks.
- database/: Folder for database interactions.
  - db.go: File for initializing and interacting with the database.
  - init.sql: SQL script to create tables.

Functionality:
- REST API for managing tasks:
  - GET /tasks: Retrieve a list of all tasks.
  - POST /tasks: Create a new task.
  - PUT /tasks/{id}: Update a task by ID.
  - DELETE /tasks/{id}: Delete a task by ID.
- Connection to a database to store task information.
- Input validation.
- Error handling and sending appropriate HTTP status codes.

Frontend (Vue.js)

Directory Structure:
- src/: Source code folder.
  - App.vue: Main application component.
  - main.js: Main JavaScript file to initialize the Vue application.
  - components/: Folder for Vue components.
    - TaskList.vue: Component to display the list of tasks.
    - TaskForm.vue: Component to add/edit tasks.

Functionality:
- Display the list of tasks.
- Form to add a new task.
- Ability to edit and delete tasks.
- Interaction with the backend through REST API.

Database (PostgreSQL)

- tasks table to store task information.

Docker / Docker Compose

- Dockerfile: To create a Docker image for our Go application.
- docker-compose.yml: To orchestrate services (Go application, database).

Getting Started

1. Clone the Repository: Clone the project repository to your local machine.
   git clone https://github.com/username/simple-to-do-list.git
   cd simple-to-do-list

2. Set Up the Backend: Navigate to the backend directory and run the Go application.
   cd backend
   go run main.go

3. Set Up the Frontend: Navigate to the frontend directory and install dependencies.
   cd frontend
   npm install
   npm run serve

4. Access the Application: Open your web browser and visit http://localhost:8080 to access the To-Do List application.

5. Using the Application: Add, edit, and delete tasks using the user interface.



