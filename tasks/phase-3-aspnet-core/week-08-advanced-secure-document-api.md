# 🛡️ Week 08 — Advanced Secure Document Management API

## 🎯 Objective

Extend the Secure Document Management API from Week 07 by adding Entity Framework Core persistence, Refresh Tokens, and Audit Logging.

## 📋 Requirements

### 1. Integrate Entity Framework Core

- Replace the in-memory data storage with Entity Framework Core.
- Persist the application data in the database.

### 2. Implement Refresh Tokens

Update the login process to return:

- A short-lived JWT Access Token (approximately 15 minutes).
- A long-lived Refresh Token (approximately 7 days).

Store Refresh Tokens in the database with:

- User ID
- Expiry date

### 3. Create Refresh Endpoint

Implement:

`POST /refresh`

The endpoint should:

- Validate the expired Access Token.
- Validate the Refresh Token.
- Return a new Access Token and Refresh Token pair when validation succeeds.

### 4. Add Department-Based Authorization

- Add a Department claim to the JWT.
- Allow users to update documents only when the Department in their JWT matches the Department of the document.

### 5. Implement Audit Logging

Create an `[AuditLog]` action filter that:

- Runs on document POST, PUT, and DELETE operations.
- Extracts the User ID from the JWT.
- Records the action in an `AuditLogs` database table.

## 🛠️ Technical Requirements

- Use Entity Framework Core for persistence.
- Store Refresh Tokens in the database.
- Use JWT claims for User ID and Department.
- Implement an action filter for audit logging.
- Store audit records in the `AuditLogs` table.

## 💡 Expected Outcome

An advanced Secure Document Management API with database persistence, Refresh Token authentication, Department-based authorization, and audit logging.
