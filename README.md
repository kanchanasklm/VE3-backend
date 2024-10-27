# 📋 TASK MANAGEMENT

This project is a web application for managing tasks, user authentication, and other functionalities. Follow the instructions below to set up and run the project.

---

## 📑 Table of Contents
1. [🔧 Prerequisites](#-prerequisites)
2. [🚀 Project Setup](#-project-setup)
   - [🐳 Docker Setup](#-docker-setup)
   - [🛠 Manual Setup](#-manual-setup)
3. [🔐 Environment Variables](#-environment-variables)
4. [📜 Database Setup](#-database-setup)
5. [📡 API Endpoints](#-api-endpoints)

---

## 🔧 Prerequisites

Ensure you have the following installed:

- *🐳 Docker* (for Docker setup)
- *🟢 Node.js* and *📦 npm* (for manual setup)
- *🛢 MySQL* (for manual setup if not using Docker)

---

## 🚀 Project Setup

### 🐳 Docker Setup

1. *📂 Clone the Repository*
   ```bash
   git clone <https://github.com/kanchanasklm/VE3-backend.git>
   cd <Assignment>

▶ Ensure Docker is Running
Make sure Docker is up and running on your machine.

🔧 Build and Start the Services
Build and start the Docker containers by running the following command:


docker compose up --build

🌐 Access the Application
Once the setup is complete, open http://localhost:3000 in your browser to view the application.

The Docker setup automatically configures a MySQL database container and an application container, running migrations to set up the database.



🛠 Manual Setup


If you prefer not to use Docker, follow these steps to set up the project manually:

📂 Clone the Repository
 git clone <https://github.com/kanchanasklm/VE3-backend.git>
   cd <Assignment>
📦 Install Dependencies
npm install

🔐 Set Up Environment Variables
Create a .env file in the root directory with the following variables:

DB_HOST=localhost
DB_PORT=3306
DB_NAME=VE3
DB_USER=host
DB_PASSWORD=1234
JWT_SECRET=mysecret
PORT=3000

🛢 Set Up MySQL Database
Ensure MySQL is running, and create a database named VE3.

▶ Run Migrations
Execute the following command to set up the database schema:

npm run migration:run

▶ Start the Application
Start the application server:

npm start

🌐 Access the Application
Open http://localhost:3000 in your browser to access the application.



📡 API Endpoints


POST /auth/login: Log in a user
POST /auth/register: Register a new user
GET /tasks: Retrieve all tasks
POST /tasks: Create a new task
PUT /tasks/
: Update a task
DELETE /tasks/
: Delete a task
