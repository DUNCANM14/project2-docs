# Project 2 – Screenshots & Explanations

This page displays all screenshots taken during development and testing of the Project 2 REST API.

---

## Docker Containers Running
Confirms the Laravel app, MySQL database, and phpMyAdmin are all running.
![Docker Containers](/data/DockerPS.png)

---

## phpMyAdmin Connected to MySQL
<<<<<<< HEAD
phpMyAdmin is successfully connected to the `project2` database, showing tables created by Laravel migrations:

=======
Shows the `project2` database and Laravel-created tables.
>>>>>>> 3569406 (Fix screenshot paths and rebuild site)
![phpMyAdmin](/data/phpMyAdmin.png)

---

## API – List Users (`GET /api/users`)
Displays JSON output from querying all users.
![GET Users](/data/GETapiusers.png)

---

## Create User (`POST /api/users`)
Valid user creation using the /api/users endpoint.
![Create User](/data/CreateUser.png)

---

## Login & Token Response (`POST /api/users/login`)
Successful login returning a Sanctum token.
![Login](/data/postlogin.png)

---

## Update Username (`PUT /api/users/{id}`)
<<<<<<< HEAD
A user successfully changed their username.  
Screenshot shows the request body and the updated response data.

=======
A user successfully updated their username.
>>>>>>> 3569406 (Fix screenshot paths and rebuild site)
![Change Username](/data/changeusername.png)

---

## Update Password (`PUT /api/users/me/password`)
<<<<<<< HEAD
A logged-in user changes their password using their Bearer token.

=======
Password successfully changed using Bearer token authentication.
>>>>>>> 3569406 (Fix screenshot paths and rebuild site)
![Password Updated](/data/password_updated.png)

---

<<<<<<< HEAD
## Running Database Migrations
Shows a successful migration inside the Docker container.

=======
## Database Migration
Shows the output of `php artisan migrate` working inside Docker.
>>>>>>> 3569406 (Fix screenshot paths and rebuild site)
![Database Migration](/data/database_migration.png)

---

<<<<<<< HEAD
## Deployment Script Output (`run.sh`)
Your deployment script executing:
=======
## Deployment Script Output
Screenshots show your automated run script performing:
- Composer install  
- Docker build & up  
- Key generation  
- Migrations  
>>>>>>> 3569406 (Fix screenshot paths and rebuild site)

![Deployment Script](/data/setuporrun.png)
![Deployment Script 2](/data/Run.png)

---

## API Tester Loaded in Browser
Your test_api.html running successfully.
![API Tester](/data/TestHTML.png)

<<<<<<< HEAD
---

# Summary
These screenshots collectively demonstrate:

- Docker environment working  
- MySQL + phpMyAdmin working  
- Full REST API functionality  
- Login + token authentication  
- All CRUD operations  
- Deployment/migration steps  
=======
>>>>>>> 3569406 (Fix screenshot paths and rebuild site)
