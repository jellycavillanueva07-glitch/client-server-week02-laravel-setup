# Client-Server Week 2 - Laravel Setup

## Introduction

### Overview of Laravel
Laravel is a powerful PHP framework designed for modern web development. It provides an elegant, expressive syntax alongside built-in tools for routing, views, authentication, and database management to streamline the creation of web applications.

### Importance of Client-Server Technologies
Client-server architecture is fundamental to modern web development. It separates the user interface (client) from the data processing and business logic (server), enabling secure, scalable, and efficient communication across web platforms.

### Purpose of the Project
This project serves as a practical setup exercise to understand the fundamentals of Laravel framework, customize views with student information, and manage version control using Git and GitHub.

## Objectives
* Successfully install and configure a new Laravel web application project.
* Modify Blade views (`welcome.blade.php`) to display custom student details.
* Set up a local development environment using PHP, Composer, and VS Code.
* Utilize Git for version control to track changes and manage commits.
* Deploy and manage the source code repository on GitHub with screenshots and documentation.

## Development Environment
* **Operating System:** Windows 11
* **PHP Version:** 8.2.x
* **Laravel Version:** 10.x / 11.x
* **Composer Version:** 2.x
* **Git Version:** 2.x
* **MySQL Version:** 8.0 / MariaDB 10.4
* **VS Code Version:** 1.8x / 1.9x

## Installation Steps
1. **Install Prerequisites:** Ensure PHP, Composer, Git, and VS Code are installed on the local system.
2. **Create Laravel Project:** Open terminal and run `composer create-project laravel/laravel hello-laravel`.
3. **Run Local Development Server:** Navigate to the project directory and execute `php artisan serve`.
4. **Customize View File:** Open `resources/views/welcome.blade.php` in VS Code and add custom student information.
5. **Capture Proof:** Take a screenshot of the running homepage and save it under the `screenshots/` directory as `homepage.png`.
6. **Initialize and Push to GitHub:** Run `git init`, commit the project files, link the remote repository using `git remote add origin`, and upload using `git push -u origin main`.

## Project Structure

* **`app/`**: Contains the core code of the application, including Controllers, Models, and Middleware.
* **`routes/`**: Contains all route definitions (such as `web.php`) that map web URLs to specific controller logic or Blade views.
* **`resources/`**: Houses views (Blade templates), uncompiled assets (CSS, JavaScript), and localization files.
* **`public/`**: Serves as the web server's document root, containing the main `index.php` entry point and compiled frontend assets (images, CSS, JS).
* **`config/`**: Contains all system configuration files for database connections, application setup, mail settings, and environment variables.
* **`database/`**: Stores database migrations, seeders, and factory files used for managing database schemas and dummy data.

## Problems Encountered and Solutions

* **Git Author Identity Unknown:**
  * *Problem:* Encountered the error `fatal: unable to auto-detect email address` when attempting to make the initial Git commit.
  * *Solution:* Executed `git config --global user.email "your-email@example.com"` and `git config --global user.name "Your Name"` to configure global credentials.

* **Incorrect Folder Naming for Screenshots:**
  * *Problem:* The screenshot folder was initially created as `screenshot/` instead of the required plural `screenshots/`, breaking image paths.
  * *Solution:* Renamed the folder to `screenshots/` in VS Code and updated the image path reference inside `README.md`.

* **Missing Project Files on Initial Remote Push:**
  * *Problem:* Only the `README.md` appeared on GitHub because the remote repository was initialized with a default file that conflicted with local commits.
  * *Solution:* Ran `git push -u origin main --force` to overwrite the remote state with the local codebase and upload all project directories.

## 10. Reflection

    Completing this project provided valuable hands-on experience in setting up a modern web application using Laravel and managing software versions with Git. Throughout the activity, I learned how client-server applications operate under the Model-View-Controller (MVC) architecture. Setting up Laravel helped me understand how server-side frameworks process requests, handle routing, and render dynamic views using Blade templates. Modifying the welcome view file reinforced my understanding of separating frontend display logic from backend configuration.

    During the development process, I encountered several technical challenges. Configuring the local environment required setting up proper system variables for PHP and Composer. Additionally, initializing Git presented authentication and branch synchronization issues when pushing the local codebase to the remote GitHub repository. Overcoming these hurdles improved my troubleshooting skills, specifically in working with CLI tools, reading terminal error messages, and executing Git commands accurately.

    Laravel plays a crucial role in modern client-server development by providing a structured, secure, and efficient framework for developers. Rather than building core components from scratch, Laravel offers built-in tools for routing, database management, authentication, and security features. This server-side architecture ensures that application logic and data processing are handled safely on the server, sending rendered HTML or structured data back to the client. Understanding this architecture is essential for building scalable, maintainable, and enterprise-grade web platforms.

    The knowledge gained from this activity will significantly benefit my future software development endeavors. Gaining proficiency in Laravel equips me with a highly sought-after skill set in full-stack web development. Furthermore, mastering Git version control establishes best practices for code management, enabling smooth collaboration in team environments. Moving forward, I can apply these client-server fundamentals to design more complex web systems, integrate database functionality, and follow industry-standard workflows.

## 11. References

* Composer. (n.d.). *Composer documentation*. https://getcomposer.org/doc/
* Git. (n.d.). *Git documentation*. https://git-scm.com/doc
* Laravel. (n.d.). *Laravel documentation*. https://laravel.com/docs
* PHP. (n.d.). *PHP manual*. https://www.php.net/manual/en/

## Homepage Preview
![Student Profile](screenshots/homepage.png)