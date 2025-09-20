# 📚 Django Book API

A simple **Book Management API** built with **Django** and **Django REST Framework (DRF)**.
It provides endpoints to **list books** and **create new books**.

## 🚀 Features

* List all books (`GET /api/books/`)
* Create a new book (`POST /api/books/create/`)
* Uses **Django REST Framework** for easy API development
* SQLite database (default, can be changed)

## ⚙️ Installation & Setup

### 1. Clone the repository

git clone https://github.com/your-username/django_api_project.git
cd django_api_project

### 2. Create and activate a virtual environment

python -m venv .venv
.venv\Scripts\activate   # On Windows
source .venv/bin/activate  # On Mac/Linux

### 3. Install dependencies

pip install django djangorestframework

### 4. Run migrations

python manage.py migrate

### 5. Start the server

python manage.py runserver

## 📖 API Endpoints

### 1. List all books

**Request**

```http
GET /api/books/
```

**Response**

```json
[
  {
    "id": 1,
    "title": "Clean Code",
    "author": "Robert C. Martin",
    "published_year": 2008
  }
]


### 2. Create a new book

**Request**

```http
POST /api/books/create/
