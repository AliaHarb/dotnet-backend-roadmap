# ✅ Week 05 — To-Do Web API

## 🎯 Objective

Build a To-Do Web API using ASP.NET Core to practice creating RESTful endpoints, dependency injection, and working with an in-memory data store.

## 📋 Requirements

### 1. Create the TodoItem Model

Create a `TodoItem` model with the following properties:

- `Id`: Generated manually by the service.
- `Title`: Required.
- `IsComplete`: Boolean value.

### 2. Create the Todo Service

Create an `ITodoService` interface with the following operations:

- Retrieve all Todo items.
- Retrieve a Todo item by ID.
- Add a new Todo item.

Implement the interface in `TodoService` using an in-memory list containing sample data.

### 3. Register the Service

- Register `TodoService` in the dependency injection container.
- Use the Singleton lifetime.

### 4. Create TodosController

Use the route:

`/api/todos`

Inject `ITodoService` into the controller and implement the following endpoints:

- **GET:** Retrieve all Todo items and return `200 OK`.
- **GET by ID:** Retrieve a Todo item by ID and return `200 OK` or `404 Not Found`.
- **POST:** Receive a Todo item as JSON, generate its ID, and return `201 Created` with the created item and its Location.

### 5. Validation and Error Handling

- Use `[ApiController]`.
- Use `[Required]` for required properties.
- Return validation errors for invalid requests.

## 🛠️ Technical Requirements

- Use an in-memory list only.
- Do not use a database or Entity Framework Core.
- Use constructor injection.
- Organize the project into:
  - Models
  - Services
  - Controllers

## 💡 Expected Outcome

A To-Do Web API with endpoints for retrieving and adding Todo items, using a service layer, dependency injection, and in-memory storage.
