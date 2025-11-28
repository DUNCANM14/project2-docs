# Project 2 – Screenshots & Explanations

This page shows the screenshots captured during development and testing of the Project 2 REST API, along with explanations of what each screenshot demonstrates.

---

## Docker Containers Running
This confirms that the application stack is running correctly:  
- **project2_app** → Laravel / PHP backend  
- **project2_mysql** → MySQL database  
- **project2_phpmyadmin** → DB dashboard

![Docker Containers](/data/DockerPS.png)

---

## phpMyAdmin Connected to MySQL
phpMyAdmin is successfully connected to the `project2` database, showing tables created by Laravel migrations:

![phpMyAdmin](/data/phpMyAdmin.png)

---

## API – List Users (`GET /api/users`)
This screenshot shows the JSON output of listing all users in the database using the API.

![GET Users](/data/GETapiusers.png)

---

## Create User (`POST /api/users`)
A successful user creation request.  
The API tester shows the JSON body used and the server response confirming creation.

![Create User](/data/CreateUser.png)

---

## Login & Token Response (`POST /api/users/login`)
Logging in returns a valid Sanctum token.  
This token is required for all protected endpoints.

![Login / Token](/data/postlogin.png)

---

## Update Username (`PUT /api/users/{id}`)
A user successfully changed their username.  
Screenshot shows the request body and the updated response data.

![Change Username](/data/changeusername.png)

---

## Update Password (`PUT /api/users/me/password`)
A logged-in user changes their password using their Bearer token.

![Password Updated](/data/password_updated.png)

---

## Running Database Migrations
Shows a successful migration inside the Docker container.

![Database Migration](/data/database_migration.png)

---

## Deployment Script Output (`run.sh`)
Your deployment script executing:

![Deployment Script](/data/setuporrun.png)
![Deployment Script 2](/data/Run.png)

---

## API Tester Loaded in Browser
The custom HTML API tester (`test_api.html`) loading correctly on port 8000.

![API Tester](/data/TestHTML.png)

---

# Summary
These screenshots collectively demonstrate:

- Docker environment working  
- MySQL + phpMyAdmin working  
- Full REST API functionality  
- Login + token authentication  
- All CRUD operations  
- Deployment/migration steps  
