# Project 2 – Screenshots & Explanations

This page displays all screenshots taken during development and testing of the Project 2 REST API.

---

## Docker Containers Running
Confirms Laravel, MySQL, and phpMyAdmin are all running.

![Docker Containers](../data/DockerPS.png)

---

## phpMyAdmin Connected to MySQL
phpMyAdmin connected to the `project2` database and shows the Laravel tables.

![phpMyAdmin](../data/phpMyAdmin.png)

---

## API – List Users (`GET /api/users`)
Shows JSON output of all users.

![GET Users](../data/GETapiusers.png)

---

## Create User (`POST /api/users`)
Successful user creation.

![Create User](../data/CreateUser.png)

---

## Login & Token Response (`POST /api/users/login`)
Successful login returning a Sanctum token.

![Login](../data/postlogin.png)

---

## Update Username (`PUT /api/users/{id}`)
A user successfully updated their username.

![Change Username](../data/changeusername.png)

---

## Update Password (`PUT /api/users/me/password`)
Password successfully changed using Bearer auth.

![Password Updated](../data/password_updated.png)

---

## Database Migration
Output from `php artisan migrate` inside Docker.

![Database Migration](../data/database_migration.png)

---

## Deployment Script Output
Your run script performing install, build, migrate, and start.

![Deployment Script](../data/setuporrun.png)
![Deployment Script 2](../data/Run.png)

---

## API Tester in Browser
Your test_api.html running correctly.

![API Tester](../data/TestHTML.png)
