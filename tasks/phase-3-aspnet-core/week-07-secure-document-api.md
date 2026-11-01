# 🔒 Week 07 — Secure Document Management API

## 🎯 Objective

Build a Secure Document Management API using ASP.NET Core and JWT Authentication, with role-based and permission-based access control.

## 📋 Requirements

### 1. Configure JWT Authentication

Configure the JWT settings:

- Issuer
- Audience
- Signing Key

### 2. Create In-Memory Users

Store users in memory with the following information:

- Id
- Username
- Password
- Role
- Permissions

### 3. Implement Authentication

Create an `AuthController` with a login endpoint:

- Accept user login credentials.
- Validate the user.
- Generate a JWT.
- Include the following claims in the token:
  - User ID
  - Role
  - Permissions

### 4. Implement Custom Permission Authorization

Create a custom `CheckPermission` attribute or filter that:

- Extracts the user ID from the JWT.
- Checks whether the user has the required permission.
- Returns `403 Forbidden` when the user does not have permission.

### 5. Create Document Endpoints

Store documents in memory with the following properties:

- ID
- Title
- Content
- Owner ID

Implement the following endpoints and authorization rules:

- **GET `/api/documents`**
  - Accessible only to Admin or Editor.

- **POST `/api/documents`**
  - Requires the `CreateDoc` permission.

- **PUT `/api/documents/{id}`**
  - Requires the `UpdateDoc` permission.

- **DELETE `/api/documents/{id}`**
  - Accessible only to Admin or the document owner.

### 6. Implement Resource-Based Authorization

- Create a `DocumentOwnerRequirement`.
- Create an authorization handler for the requirement.
- Define a `DocumentOwnerOrAdmin` authorization policy.
- Register the policy in the application.

### 7. Test the API

Use Swagger or Postman to test the endpoints and authorization rules.

Verify that:

- Unauthenticated requests return `401 Unauthorized`.
- Authenticated users without the required permissions receive `403 Forbidden`.
- Missing documents are handled correctly.

## 💡 Expected Outcome

A Secure Document Management API with JWT authentication, role-based authorization, custom permission checks, and resource-based authorization for document ownership.
