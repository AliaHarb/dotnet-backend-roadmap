# 📘 Week 02 — Student & Course Management

## 🎯 Objective

Upgrade the existing Student Management project by adding Course Management and connecting students to courses using Entity Framework Core and SQL Server.

## 📋 Requirements

### 1. Course Management

Create a `Course` model with the following properties:

- CourseId
- CourseName
- CourseCode
- Credits
- Description

Implement the following CourseController actions:

- Index
- Details
- Create
- Edit
- Delete

### 2. Student-Course Relationship

- Add `CourseId` as a foreign key to the Student model.
- Add a navigation property connecting Student to Course.
- Allow a Student to be linked to a Course.

### 3. Update Student Operations

- Add a Course dropdown to the Student Create view.
- Add a Course dropdown to the Student Edit view.
- Display the student's Course in the Student Details view.

## 🛠️ Technical Requirements

- Use Entity Framework Core.
- Use SQL Server.
- Create an `ApplicationDbContext`.
- Apply the Code First approach.
- Create and apply database migrations.
- Implement CRUD operations for Courses.

## 💡 Expected Outcome

An extended Student Management MVC application with Course Management and a relationship between Students and Courses, persisted using EF Core and SQL Server.
