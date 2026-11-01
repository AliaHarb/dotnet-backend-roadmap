# 🛠️ Week 03 — Validation & Repository Pattern

## 🎯 Objective

Refactor the existing Student Management System by adding validation and applying the Repository Pattern to separate data access from the controller.

## 📋 Requirements

### 1. Add Model Validation

Apply the following validation rules to the Student model:

- **Name**
  - Required.
  - Maximum length: 50 characters.
  - Minimum length: 3 characters.

- **Email**
  - Required.
  - Must be a valid email address.

- **Age**
  - Must be between 18 and 60.

### 2. Display Validation Messages

- Display validation messages in the Create and Edit views.
- Enable client-side validation.

### 3. Create Custom Unique Email Validation

- Create a custom `UniqueEmail` validation attribute.
- Prevent adding a Student with an email that already exists in the database.

### 4. Implement Repository Pattern

Create an `IStudentRepository` interface with the following methods:

- `GetAll`
- `GetById`
- `Add`
- `Update`
- `Delete`

Implement the interface in `StudentRepository` using `AppDbContext`.

### 5. Refactor StudentController

- Remove direct `AppDbContext` usage from the controller.
- Inject `IStudentRepository` into the controller.
- Register the repository with a scoped lifetime in `Program.cs`.

## 🎁 Bonus

Use Session to track the last 3 visited students and display them on the Index page under a **Recently Viewed** section.

## 💡 Expected Outcome

A refactored Student Management System with model validation, custom unique email validation, and a Repository Pattern implementation that separates data access from the controller.
