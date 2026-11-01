# 🔐 Week 04 — Secure Student Management MVC

## 🎯 Objective

Secure the existing Student Management MVC application using ASP.NET Core Identity and role-based authorization.

## 📋 Requirements

### 1. Implement ASP.NET Core Identity

- Configure ASP.NET Core Identity.
- Create an `AccountController`.
- Implement the following actions:
  - Register
  - Login
  - Logout

### 2. Update Navigation

- For anonymous users, show Register and Login.
- For authenticated users, show Logout and the username.

### 3. Implement Role-Based Authorization

Create the following roles:

- **Admin:** Has full CRUD permissions.
- **User:** Has read-only access.

Apply authorization rules to the relevant controllers and actions.

### 4. Handle Anonymous Access

- Redirect anonymous users to the Login page when they try to access protected actions.

### 5. Preserve Existing Features

- Keep the Repository Pattern implementation.
- Keep the existing validation rules.

## 🎁 Bonus

Add a `CreatedBy` property to store the email of the logged-in Admin who created the Student.

## 📦 Submission

Submit the complete GitHub repository, including:

- DbContext configured with Identity.
- AccountController and its views.
- Secured controllers.
- Repository implementation.
- Database migrations.

## 💡 Expected Outcome

A secured Student Management MVC application using ASP.NET Core Identity, with Admin and User roles and the required authorization rules.
