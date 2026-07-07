# Human Resource Management System

A full-stack Human Resource Management System built using React, Tailwind CSS, Node.js, Express, and MySQL.

The system centralizes employee onboarding, attendance tracking, leave management, salary visibility, and role-based access for administrators, HR personnel, and employees.

This project was developed as a working prototype to replace disconnected spreadsheets and manual HR workflows with one centralized platform.

---

## Project Overview

The HRMS platform provides two role-based portals:

- Admin / HR Portal
- Employee Portal

Admins and HR personnel can manage employees, monitor attendance, review leave requests, and manage salary structures.

Employees can securely log in to view their profile, attendance history, leave requests, and salary details.

---

## Implemented Features

- Role-based authentication
- Employee onboarding
- Automatic employee ID generation
- Temporary password generation
- Mandatory password change after first login
- Employee profile management
- Attendance check-in and check-out
- Attendance history and date filtering
- Leave request and approval workflow
- Salary structure and allowance visibility
- Salary history preservation
- Admin and HR dashboards
- Employee dashboard
- Protected frontend and backend routes

---

## Tech Stack

### Frontend

- React
- Vite
- Tailwind CSS
- React Router
- Font Awesome
- Fetch API

### Backend

- Node.js
- Express.js
- MySQL
- mysql2
- JSON Web Token
- bcryptjs
- dotenv
- cors

---

## Main Features

### Authentication and Role-Based Access

- Secure login using employee ID or email
- JWT-based authentication
- Password hashing using bcrypt
- Protected frontend and backend routes
- Role-based authorization for:
  - Admin
  - HR
  - Employee
- Forced password change after first login for newly created employees

---

## Admin / HR Features

### Employee Management

- View all employees
- Search employees by name, employee ID, department, designation, or role
- Create new employee accounts
- Automatically generate unique employee IDs
- Generate temporary employee passwords
- View detailed employee profiles
- View employee department, role, designation, employment type, and joining date

### Employee ID Generation

Employee IDs are generated automatically using the following format:

```text
OI + first two letters of first name + first two letters of last name + joining year + yearly sequence
