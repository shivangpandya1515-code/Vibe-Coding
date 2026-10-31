# 🚀 Practical-9: Laravel Application Deployment Using SSH

<p align="center">
  <img src="https://img.shields.io/badge/Laravel-13.39.0-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel">
  <img src="https://img.shields.io/badge/PHP-8.5.0-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP">
  <img src="https://img.shields.io/badge/Composer-2.8.12-885630?style=for-the-badge&logo=composer&logoColor=white" alt="Composer">
  <img src="https://img.shields.io/badge/SSH-Enabled-000000?style=for-the-badge&logo=openssh&logoColor=white" alt="SSH">
</p>

## 🧪 Experiment Title

**Deployment and Configuration of a Laravel Web Application on an SSH-Based Hosting Environment**

## 🎯 Objective

To understand and implement the deployment and configuration of a Laravel web application using SSH (Secure Shell), including connecting to a local SSH server, checking the PHP and Composer environments, executing Laravel commands, running database migrations, and starting the Laravel development server.

## 📖 Introduction

SSH (Secure Shell) is a network protocol that provides a secure way to access and manage another computer remotely through a command-line interface.

Laravel is a PHP-based web application framework used to develop modern and dynamic web applications.

In this practical, a Laravel application is accessed and managed through an SSH connection to the local Windows machine. PHP, Composer, and Laravel commands are executed through SSH, and the Laravel development server is started to verify that the application is running successfully.

**Note:** This practical demonstrates SSH-based deployment and execution in a local environment using `localhost`. It is not a deployment to a public hosting provider.

## 🛠️ Technologies & Tools Used

| Technology / Tool | Purpose |
|---|---|
| Laravel 13.39.0 | PHP web application framework |
| PHP 8.5.0 | Server-side programming language |
| Composer 2.8.12 | PHP dependency manager |
| OpenSSH | Secure remote command execution |
| Windows PowerShell | Command-line interface |
| SQLite / Configured Database | Database management |
| Visual Studio Code | Code editing |
| Google Chrome | Testing the application |

## 📂 Project Structure

```text
Practical-9/
│
├── laravel-app/
│   ├── app/
│   ├── bootstrap/
│   ├── config/
│   ├── database/
│   ├── public/
│   ├── resources/
│   ├── routes/
│   ├── storage/
│   ├── tests/
│   ├── vendor/
│   ├── artisan
│   ├── composer.json
│   ├── package.json
│   └── .env
│
├── .gitignore
└── README.md
```

*The screenshots folder should contain your actual practical screenshots. The filenames above are suggested examples.*

## ⚙️ Requirements

Before starting the practical, ensure the following are installed and configured:

- Windows 10/11
- PHP 8.5.0
- Composer 2.8.12
- Laravel 13.39.0
- OpenSSH Client and Server
- Visual Studio Code
- Google Chrome or another web browser

## 🔧 Implementation Steps

### Step 1: Configure the SSH Environment

Open Windows PowerShell and navigate to your Practical-9 folder:

```powershell
cd "$env:USERPROFILE\OneDrive\Desktop\Vibe Coding\Practical-9"
```

Connect to the local SSH server:

```powershell
ssh localhost
```

Enter your Windows account password when prompted.

### Step 2: Verify PHP Installation

Execute the following command through SSH:

```powershell
ssh localhost "php -v"
```

Expected output:

```text
PHP 8.5.0 (cli)
```

### Step 3: Verify Composer Installation

Execute:

```powershell
ssh localhost "composer --version"
```

Expected output:

```text
Composer version 2.8.12
```

### Step 4: Verify Laravel Installation

Navigate to your Laravel application directory through SSH and check the framework version:

```powershell
ssh localhost "cd C:\path\to\laravel-app && php artisan --version"
```

Replace `C:\path\to\laravel-app` with the actual absolute path of your Laravel application.

Expected output:

```text
Laravel Framework 13.39.0
```

### Step 5: Check Database Migrations

Run the following command:

```powershell
ssh localhost "cd C:\path\to\laravel-app && php artisan migrate:status"
```

This command displays the database migration status.

Expected result:

```text
create_users_table     [1] Ran
create_cache_table     [1] Ran
create_jobs_table      [1] Ran
```

### Step 6: Start the Laravel Development Server

Execute the following command:

```powershell
ssh localhost "cd C:\path\to\laravel-app && php artisan serve --host=0.0.0.0 --port=8000"
```

Expected output:

```text
INFO  Server running on [http://0.0.0.0:8000].

Press Ctrl+C to stop the server.
```

Keep the PowerShell window open while the server is running.

### Step 7: Open the Application in Browser

Open Google Chrome and visit:

```text
http://127.0.0.1:8000
```

The Laravel welcome page should appear in the browser.

This confirms that the Laravel application is running successfully.

### Step 8: Stop the Server

To stop the Laravel development server, return to PowerShell and press:

```text
Ctrl + C
```

## 📸 Screenshots

Add your actual practical screenshots inside the `screenshots/` folder.

Recommended screenshots:

1. SSH connection with localhost.
2. PHP version verification.
3. Composer version verification.
4. Laravel framework version verification.
5. Successful database migrations.
6. Laravel development server running.
7. Laravel welcome page displayed in the browser.

## ✅ Expected Outcome

- Successfully configured and accessed the local SSH environment.
- Verified PHP and Composer installations through SSH.
- Checked the Laravel framework version.
- Executed Laravel Artisan commands remotely through SSH.
- Verified database migration status.
- Started the Laravel development server.
- Successfully accessed the Laravel application through a web browser.

## 📊 Experiment Result & Analysis

The practical was successfully completed by configuring and using an SSH connection to access the local Windows environment.

PHP 8.5.0, Composer 2.8.12, and Laravel Framework 13.39.0 were successfully verified. Database migrations were executed successfully, and the Laravel development server started on port 8000.

The Laravel welcome page was displayed successfully in the browser using `http://127.0.0.1:8000`.

This practical helped in understanding SSH-based command execution, Laravel application configuration, database migration management, and web server execution.

## 🔐 Security Considerations

- Never share your Windows account password or SSH credentials.
- Keep the Laravel `.env` file private.
- Do not upload sensitive credentials to GitHub.
- Use secure SSH authentication.
- For real production deployment, configure a production web server, HTTPS, environment variables, and proper file permissions.

## 👨‍🎓 Student Details

| Field | Details |
|---|---|
| Student Name | Shivang Pandya |
| Course | Diploma in Computer Science Engineering |
| Semester | 5th Semester |
| Subject | Vibe Coding |
| Practical Number | 09 |
| College | Shree Labhubhai Trivedi Institute of Engineering and Technology |
| College Code | 954 |

## 🏁 Conclusion

This practical demonstrated how to access and manage a Laravel application through SSH. PHP, Composer, Laravel, database migrations, and the development server were successfully verified and executed.

The experiment provided practical knowledge of SSH connections, command-line application management, and the basic process of deploying and running a Laravel web application in a local SSH-based environment.

---

<p align="center">
  <b>🎓 Diploma 5th Semester | Computer Science Engineering</b><br>
  <b>Practical-9 | Vibe Coding</b>
</p>