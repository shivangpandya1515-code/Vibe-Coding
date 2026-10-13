# 🚀 Practical-8: Laravel CRUD Application Using AI-Assisted Code Generation

<p align="center">
  <img src="https://img.shields.io/badge/Laravel-13.x-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel">
  <img src="https://img.shields.io/badge/PHP-8.5-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP">
  <img src="https://img.shields.io/badge/Database-SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" alt="SQLite">
  <img src="https://img.shields.io/badge/UI-Bootstrap_5-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white" alt="Bootstrap">
</p>

## 📌 Experiment Details

**Experiment Title:** Developing a Laravel CRUD Application Using AI-Assisted Code Generation

**Objective:** To develop Create, Read, Update, and Delete (CRUD) functionality in Laravel by using AI prompts to generate and modify application code.

## 📖 Introduction

This practical demonstrates the development of a Student Management System using the Laravel PHP framework. AI-assisted coding is used to help generate, understand, and modify application code for implementing CRUD operations.

The application allows users to add new students, view student records, update existing information, and delete records. Laravel Eloquent ORM is used for database operations, SQLite is used for data storage, and Bootstrap is used to create a clean user interface.

## 🎯 Objectives

- Understand the fundamentals of the Laravel framework.
- Learn how to use AI prompts for code generation and modification.
- Implement CRUD operations using Laravel controllers and models.
- Integrate an SQLite database with a Laravel application.
- Create dynamic web pages using Laravel Blade templates.
- Apply form validation and basic database constraints.
- Test the application through a web browser.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| PHP 8.5 | Server-side programming |
| Laravel 13 | Web application framework |
| SQLite | Database management |
| Eloquent ORM | Database interaction |
| Blade Templates | Dynamic HTML rendering |
| Bootstrap 5 | Responsive user interface |
| Composer | PHP dependency management |
| Visual Studio Code | Code editor |
| AI Coding Assistant | Code generation, explanation, and debugging |

## ✨ Features

- ➕ **Create:** Add a student with name, email, and course.
- 📋 **Read:** Display all student records in a table.
- ✏️ **Update:** Edit existing student information.
- 🗑️ **Delete:** Remove a student record after confirmation.
- ✅ **Validation:** Validate required fields and email uniqueness.
- 💾 **Database Integration:** Store student data in SQLite.
- 🎨 **Responsive UI:** Use Bootstrap styling for the interface.
- 🤖 **AI-Assisted Development:** Generate and improve code using AI prompts.

## 📂 Project Structure

```text
Practical-8/
├── app/
│   ├── Http/
│   │   └── Controllers/
│   │       └── StudentController.php
│   └── Models/
│       └── Student.php
├── bootstrap/
├── config/
├── database/
│   ├── migrations/
│   │   └── create_students_table.php
│   └── database.sqlite
├── public/
├── resources/
│   └── views/
│       └── students/
│           ├── index.blade.php
│           ├── create.blade.php
│           └── edit.blade.php
├── routes/
│   └── web.php
├── tests/
├── .env.example
├── .gitignore
├── artisan
├── composer.json
├── composer.lock
├── package.json
└── README.md
```

*Note: Laravel-generated migration filenames contain timestamps. The structure above shows the main files relevant to this practical.*

## ⚙️ Installation and Configuration

### 1. Prerequisites

Ensure the following software is installed:

- PHP
- Composer
- Visual Studio Code or another code editor
- A web browser

### 2. Open the Project Directory

```bash
cd Practical-8
```

### 3. Install Dependencies

```bash
composer install
```

### 4. Configure the Environment

If `.env` does not exist, create it from the example file.

Windows PowerShell:

```powershell
Copy-Item .env.example .env
```

Generate the application key:

```bash
php artisan key:generate
```

### 5. Configure SQLite

Ensure the following settings are present in `.env`:

```env
DB_CONNECTION=sqlite
```

Make sure the SQLite database file exists at:

```text
database/database.sqlite
```

If it does not exist, create an empty file at that location. If Laravel is already configured and working with SQLite, retain the existing configuration.

### 6. Run Database Migrations

```bash
php artisan migrate
```

This command creates the required database tables, including the `students` table.

## ▶️ Running the Application

Start the Laravel development server:

```bash
php artisan serve
```

Open the following URL in your browser:

**http://127.0.0.1:8000**

The Student Management System page will display the student table and an **Add Student** button.

## 🧪 Testing CRUD Operations

### 1. Create a Student

- Click **Add Student**.
- Enter the student's name, email, and course.
- Click **Save Student**.
- Verify that the record appears in the table.

### 2. Read Student Records

- Open the home page.
- Verify that saved students and their details are displayed.

### 3. Update a Student

- Click **Edit** beside a student record.
- Modify the required information.
- Click **Update Student**.
- Verify that the updated information appears in the table.

### 4. Delete a Student

- Click **Delete** beside a student record.
- Confirm the deletion.
- Verify that the record is removed from the table.

## 🤖 AI-Assisted Code Generation

AI-assisted development can be performed using prompts such as:

**Prompt 1 — Model and Migration**

> Generate a Laravel Student model and migration with name, unique email, course, and timestamps.

**Prompt 2 — CRUD Controller**

> Generate a Laravel resource controller that implements create, read, update, and delete operations for students using Eloquent ORM and validation.

**Prompt 3 — Blade Views**

> Generate Bootstrap-based Laravel Blade templates for listing students, adding a student, and editing student details.

**Prompt 4 — Debugging**

> Analyze the Laravel error, identify its cause, and suggest a correction compatible with the current Laravel version.

AI-generated code should always be reviewed, tested, and modified as necessary before use.

## 🔐 Important Notes

- Do not upload `.env` or sensitive credentials to a public repository.
- Keep `vendor/` and `node_modules/` out of version control.
- The SQLite database file is excluded from GitHub in this project's `.gitignore`; recreate it and run migrations when setting up a fresh copy.
- Keep `.env.example` in the repository without private credentials.
- Use this development server for local testing, not production deployment.

## 📚 Learning Outcomes

After completing this practical, the learner should be able to:

- Explain Laravel's MVC architecture.
- Create and configure models, migrations, and controllers.
- Perform CRUD operations using Eloquent ORM.
- Build dynamic interfaces using Blade templates.
- Integrate SQLite with Laravel.
- Use AI prompts to generate, explain, and debug application code.
- Test and troubleshoot a basic web application.

## ✅ Result

A Student Management System was developed using Laravel with SQLite database integration. The application implements Create, Read, Update, and Delete operations through a Bootstrap-based interface. AI-assisted code generation was used to support the development and modification of application components.

**Practical-8 successfully demonstrates Laravel CRUD development using AI-assisted coding techniques.**

---

<p align="center">
  <b>🎓 Practical-8 | Vibe Coding</b><br>
  Built with Laravel, PHP, SQLite, Bootstrap, and AI-assisted development.
</p>