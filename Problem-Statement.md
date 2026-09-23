# Library Management System

## 1. Resource Planning & Utilization Queries

- Identify duplicate or suspicious student identity records to help detect unauthorized use of identities.
- Identify peak library hours.
- Determine how many students use the library during their free periods.
- Identify the most frequent library visitors.
- Analyze the purpose of library visits, such as borrowing books, returning books, reading/studying, or other activities.
- Identify the most demanded book in each library section.
- Identify overdue books and the students who have not returned them by the due date.

## 2. Database Design

Based on the identified requirements and queries, a relational database needs to be designed to store and manage information about students, books, sections, library visits, book transactions, and other relevant entities.

### Requirements and Corresponding Tables

| Requirement | Required Table(s) |
|---|---|
| Fake/duplicate identity | Student |
| Peak library hours | Library_Visit |
| Free-period usage | Library_Visit, Student |
| Frequent visitors | Library_Visit, Student |
| Visit purpose | Library_Visit |
| Most demanded books in each section | Book, Section, Book_Transaction |
| Overdue books | Book_Transaction, Fine, Student |

The database should define appropriate tables, attributes, primary keys, foreign keys, relationships, and constraints.

The main tables proposed for the system are:

- Student
- Book
- Section
- Author
- Publisher
- Library_Visit
- Book_Transaction
- Fine

## 3. User-specific Views

The system should provide appropriate database views for different types of users, such as students, librarians, and administrators. Each user should be able to access information relevant to their role while maintaining appropriate data visibility.

## 4. Triggers, Procedures and Functions

The system should use triggers, stored procedures, and functions to handle important database operations and automatic updates. These may include updating book availability after issue or return, calculating fines for overdue books, maintaining visit records, and ensuring data consistency during updates.

## Overall Objective

The overall objective is to develop a Library Management System that can efficiently manage library data, support resource planning and utilization, provide role-specific information, and automate important database operations.
