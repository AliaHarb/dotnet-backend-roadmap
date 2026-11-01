# 📦 Week 06 — Product Management API

## 🎯 Objective

Build a Product Management API using ASP.NET Core and Entity Framework Core to practice CRUD operations, service-layer separation, action filters, configuration, and logging.

## 📋 Requirements

### 1. Create the Product Model

Create a `Product` model with the following properties:

- Id
- Name
- Description
- Price
- Stock

### 2. Implement CRUD Endpoints

The API should support:

- **GET:** Retrieve all products.
- **GET by ID:** Retrieve a specific product.
- **POST:** Create a new product.
- **PUT:** Update an existing product.
- **DELETE:** Delete a product.

### 3. Implement Product Service

- Create a `ProductService` to handle business logic.
- Register the service using Dependency Injection.
- Keep business logic separate from the controller.

### 4. Add Custom Action Filter

Create a custom action filter for one of the following purposes:

- Log execution time.
- Validate product price.

### 5. Configuration and Logging

- Use `IConfiguration` to read application settings from `appsettings.json`.
- Use `ILogger` to log product creation, updates, and deletions.

### 6. Request Binding

Practice using:

- `[FromRoute]`
- `[FromQuery]`
- `[FromBody]`

### 7. Response Status Codes

Handle the appropriate response status codes:

- `200 OK`
- `201 Created`
- `204 No Content`
- `404 Not Found`

### 8. DTOs

Create DTOs for:

- Creating a product.
- Updating a product.
- Returning product data.

## 🛠️ Technical Requirements

- Use Entity Framework Core.
- Use SQL Server.
- Configure the DbContext.
- Apply the Code First approach.
- Create and apply database migrations.
- Ensure product data persists after the application restarts.

## 💡 Expected Outcome

A Product Management API with persistent SQL Server storage, CRUD endpoints, a separate service layer, custom action filter, configuration, logging, and DTOs.
