# CRUD Inventory Prototype (FastAPI)

*A prototype inventory management system built with FastAPI, focused on CRUD (Create, Read, Update, Delete) operations for managing inventory items and users with authentication.*

## Features

- Add new inventory items with validation using **Pydantic**
- View all items with filtering and sorting options
- Update existing items with validation and error handling
- Delete items with confirmation and error handling
- Powered by **FastAPI** for quick development and testing
- User authentication using **OAuth2** and **JWT** tokens
- Password hashing using **Passlib** and **Bcrypt**

## Tech Stack

| Layer | Technology |
|---|---|
| Web framework | FastAPI |
| Validation | Pydantic |
| ORM | SQLAlchemy |
| Database | SQLite |
| ASGI server | Uvicorn |
| Auth | OAuth2, JWT (`python-jose`, `pyjwt`) |
| Password hashing | Passlib + Bcrypt |
| Testing | pytest, httpx |
| Tooling | Black, isort, mypy, vulture |

Dependency management is via `Pipfile` (Python 3.8).

## Getting Started

### Prerequisites

- Python 3.8
- [pipenv](https://pipenv.pypa.io/) (dependencies are declared in `Pipfile`)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/gokulKumbakkara/Inventory-Application-Prototype.git
   ```
2. Install the required dependencies:
   ```bash
   pipenv install
   ```

## Usage

To run the application, navigate to the project directory and run:
```bash
uvicorn main:app --host 0.0.0.0 --port 8000
```
This starts the Uvicorn server and makes the API available at `http://localhost:8000`.

## Project Structure

- `models/` — database models and schema definitions
- `repository/` — database repository layer for interacting with the database
- `routers/` — API routers for handling requests and responses
- `schema/` — API schema definitions using Pydantic
- `security/` — security-related functionality, including authentication and authorization
- `tests/` — unit tests and integration tests for the application

## Contributing

To contribute to this project, please fork the repository and submit a pull request with your changes. Make sure to include unit tests and integration tests for any new functionality. The project uses **Black** for code formatting, **Isort** for import sorting, and **Mypy** for type checking. Please ensure that your code conforms to these standards.
