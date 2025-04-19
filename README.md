# ✅ FastAPI To-Do List with MySQL

A full-featured **To-Do List REST API** built using **FastAPI**, **MySQL**, and **JWT Authentication**. This project demonstrates building secure, production-ready APIs with database integration, user auth, and Alembic migrations.

---

## 🚀 Features

- User Registration & JWT-based Login Authentication
- Secure Route Protection with Bearer Tokens
- Create, Read, Update, and Delete (CRUD) Tasks
- Task Filtering (by status, priority)
- Task Sorting (by id, due_date, priority)
- Pagination Support
- MySQL Database Integration via SQLAlchemy ORM
- Alembic for Database Migrations
- `.env` for Secret Management
- Postman Collection for API Testing

---

## 🔧 Tech Stack

- **FastAPI**
- **MySQL**
- **SQLAlchemy**
- **Pydantic**
- **JWT (via PyJWT)**
- **Alembic**
- **Python 3.11**
- **Postman** for testing

---

## 📁 Project Structure

fastapi_to_do_list/ │ 
├── todo_App/ │
├── auth/ # JWT auth logic │
├── routes/ # API routes (task_routes) │ 
├── models.py # SQLAlchemy models │ 
├── schema.py # Pydantic schemas │ 
├── database.py # DB session + engine │ 
├── main.py # FastAPI app entry point │ 
├── .env # Environment variables ├── alembic/ # Migration files 
├── requirements.txt 
├── README.md 
└── .gitignore

## 🧠 Database Setup (MySQL)

Run this query in your MySQL client to create the database:

```sql
CREATE DATABASE todo_db;
USE todo_db;
```

🔄 Alembic Migrations (TL;DR)

alembic init alembic
# Configure alembic.ini and env.py
alembic revision --autogenerate -m "create tasks table"
alembic upgrade head


🔐 Authentication
Register: /auth/register

Login: /auth/login

Use the returned access_token in headers:
->Authorization: Bearer <your_token_here>


🔥 Sample Task Endpoints

Method	Endpoint	Description
POST	/tasks/	Create a new task
GET	/tasks/	Get all tasks
GET	/tasks/{id}	Get a single task
PUT	/tasks/{id}	Update a task
DELETE	/tasks/{id}	Delete a task



🧪 .env Sample

SECRET_KEY=mysecretkey
DATABASE_URL=mysql+mysqlconnector://root:yourpassword@localhost/todo_db




## ⭐ Support
If you find this project useful, consider giving it a ⭐ on GitHub. It helps others find it too!




👤 Author
Abhishek Kumar
💼 Python Developer | FastAPI | Django | MySQL | DRF | Wagtail
📧 Connect on LinkedIn
- 🔗 [LinkedIn Profile](https://www.linkedin.com/in/abhishek-kumar-294650205/)
- 📫 Email: abhishek.xyz878@gmail.com
