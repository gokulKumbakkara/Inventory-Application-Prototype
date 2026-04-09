# 📦 CRUD Inventory Prototype (FastAPI)
This project is a **prototype inventory management system** built with **FastAPI**, focusing on building and understanding **CRUD (Create, Read, Update, Delete)** operations for managing inventory items and users with authentication.

## 🚀 Features
- ➕ Add new inventory items with validation using **Pydantic**
- 📋 View all items with filtering and sorting options
- ✏️ Update existing items with validation and error handling
- ❌ Delete items with confirmation and error handling
- ⚡ Powered by **FastAPI** for quick development and testing
- 🔒 User authentication using **OAuth2** and **JWT** tokens
- 🔑 Password hashing using **Passlib** and **Bcrypt**

## 🛠️ Tech Stack
- **FastAPI** → Web framework for building the API
- **Pydantic** → Data validation and serialization
- **SQLAlchemy** → Database ORM for interacting with the database
- **SQLite** → Database storage for the prototype
- **Uvicorn** → ASGI server for running the application
- **Passlib** and **Bcrypt** → Password hashing and verification
- **PyJWT** → JSON Web Token handling for authentication

## 📦 Installation
To install the required dependencies, run the following command:
```bash
pip install -r Pipfile
```
This will install all the dependencies specified in the `Pipfile`.

## 🚀 Usage
To run the application, navigate to the project directory and run the following command:
```bash
uvicorn main:app --host 0.0.0.0 --port 8000
```
This will start the Uvicorn server and make the API available at `http://localhost:8000`.

## 📂 Folder Structure
The project is organized into the following folders:
- `models`: Database models and schema definitions
- `repository`: Database repository layer for interacting with the database
- `routers`: API routers for handling requests and responses
- `schema`: API schema definitions using **Pydantic**
- `security`: Security-related functionality, including authentication and authorization
- `tests`: Unit tests and integration tests for the application

## 🤝 Contributing
To contribute to this project, please fork the repository and submit a pull request with your changes. Make sure to include unit tests and integration tests for any new functionality. The project uses **Black** for code formatting, **Isort** for import sorting, and **Mypy** for type checking. Please ensure that your code conforms to these standards.