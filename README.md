# Employee API

A RESTful Employee Management API built with **Java**, **Spring Boot**, and **Gradle**.

This project demonstrates a clean backend structure for managing employee data through standard CRUD operations and RESTful endpoints.

## Features

- Create employee records
- Retrieve all employees
- Retrieve an employee by ID
- Update employee information
- Delete employee records
- RESTful API design
- Gradle-based build system
- Spring Boot project structure

## Tech Stack

- Java
- Spring Boot
- Spring Web
- Gradle
- REST API
- JSON

## Project Structure

```text
employee-api/
├── gradle/
├── src/
│   ├── main/
│   │   ├── java/
│   │   └── resources/
│   └── test/
├── .gitattributes
├── .gitignore
├── build.gradle
├── gradlew
├── gradlew.bat
├── HELP.md
└── settings.gradle
```

## Prerequisites

Before running the application, make sure you have:

- Java installed
- Git installed

You do not need to install Gradle separately because the project includes the Gradle Wrapper.

Check your Java installation:

```bash
java -version
```

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/employee-api.git
cd employee-api
```

Replace `YOUR_USERNAME` with your GitHub username.

### 2. Build the Application

#### macOS / Linux

```bash
./gradlew build
```

#### Windows

```bash
gradlew.bat build
```

### 3. Run the Application

#### macOS / Linux

```bash
./gradlew bootRun
```

#### Windows

```bash
gradlew.bat bootRun
```

By default, the application runs at:

```text
http://localhost:8080
```

## API Endpoints

The API follows a standard employee CRUD pattern.

| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/employees` | Create a new employee |
| `GET` | `/employees` | Retrieve all employees |
| `GET` | `/employees/{id}` | Retrieve an employee by ID |
| `PUT` | `/employees/{id}` | Update an existing employee |
| `DELETE` | `/employees/{id}` | Delete an employee |

> If your controller uses a different base path, update the endpoint table to match the implementation.

## Example Request

Example employee payload:

```json
{
  "name": "John Doe",
  "email": "john.doe@example.com",
  "department": "Engineering"
}
```

## Example Response

```json
{
  "id": 1,
  "name": "John Doe",
  "email": "john.doe@example.com",
  "department": "Engineering"
}
```

## Useful Gradle Commands

Build the project:

```bash
./gradlew build
```

Run the application:

```bash
./gradlew bootRun
```

Run tests:

```bash
./gradlew test
```

Clean generated build files:

```bash
./gradlew clean
```

Clean and rebuild:

```bash
./gradlew clean build
```

On Windows, replace `./gradlew` with `gradlew.bat`.

## Typical Application Architecture

```text
Client
  |
  v
Controller
  |
  v
Service
  |
  v
Repository
  |
  v
Database
```

A typical Spring Boot application separates responsibilities into:

- **Controller** — receives HTTP requests and returns responses
- **Service** — contains business logic
- **Repository** — handles persistence and database access
- **Model / Entity** — represents application data

## Testing

Run the test suite with:

```bash
./gradlew test
```

Test reports are generated under:

```text
build/reports/tests/test/
```

## Future Improvements

Possible enhancements include:

- PostgreSQL or MySQL integration
- Spring Data JPA
- Request validation
- Global exception handling
- Swagger / OpenAPI documentation
- Unit and integration tests
- Docker support
- JWT authentication
- Role-based authorization
- GitHub Actions CI/CD
- Logging and monitoring

## Learning Objectives

This project demonstrates:

- Java backend development
- Spring Boot fundamentals
- REST API design
- CRUD operations
- HTTP methods and status handling
- JSON request and response handling
- Gradle dependency and build management
- Layered backend architecture

## License

This project is intended for learning and portfolio purposes.
