# 🔗 Week 12 — EF Core Advanced

## 🎯 Objective

Extend the Employee & Project Management System from Week 11 by implementing entity relationships and handling related data using Entity Framework Core.

## 📋 Requirements

### 1. Define Entity Relationships

- **Department and Employee**
  - One Department can have many Employees.
  - Each Employee belongs to one Department.

- **Employee and Project**
  - An Employee can be assigned to multiple Projects.
  - A Project can have multiple Employees.

### 2. Manage Relationships

The application should allow users to:

- Assign an Employee to a Department.
- Change an Employee's Department.
- Assign Projects to an Employee.
- Remove Projects from an Employee.
- Display related details for each entity.

### 3. Handle Related Data

- Use navigation properties.
- Use `Include` to retrieve related data.
- Configure foreign keys and navigation properties.
- Apply the required database migrations.

### 4. Improve the User Experience

- Show existing data when editing a record.
- Do not expose database IDs as user choices.
- Display numbered options and names instead.
- Handle invalid selections.
- Prevent deleting records when invalid relationships exist.

## 🛠️ Technical Requirements

- Use Entity Framework Core.
- Implement one-to-many and many-to-many relationships.
- Use foreign keys and navigation properties.
- Use `Include` when retrieving related data.
- Apply migrations to update the database schema.

## 💡 Expected Outcome

An extended Employee & Project Management System that handles entity relationships and related data correctly, with user-friendly selection and validation.
