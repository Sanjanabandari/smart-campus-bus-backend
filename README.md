# Smart Campus Bus Management System — Backend

A Spring Boot REST API for managing campus transportation data. The backend provides CRUD operations for buses, routes, drivers, students, and schedules, with MySQL as the database.

## Features

- **Bus Management:** Add, view, update, and delete bus records.
- **Route Management:** Manage route names, starting points, destinations, and stops.
- **Driver Management:** Store driver details, phone numbers, license numbers, and addresses.
- **Student Management:** Manage student names, roll numbers, departments, phone numbers, and years.
- **Schedule Management:** Manage bus numbers, routes, departure times, arrival times, and days.
- **Database Integration:** Store and retrieve records using MySQL.

## Technologies Used

- Java 17
- Spring Boot
- Spring Data JPA
- Hibernate
- MySQL 8
- Maven
- REST API

## Prerequisites

Install the following software before running the backend:

- Java 17 or later
- MySQL Server 8
- Maven, or use the included Maven Wrapper

## Database Configuration

Create the database in MySQL:

```sql
CREATE DATABASE campus_bus;
```

Configure the database connection in `src/main/resources/application.properties`.

Set your database URL, username, and password using environment variables:

- `DB_URL`
- `DB_USERNAME`
- `DB_PASSWORD`

Do not upload database passwords or other secrets to GitHub.

## Run the Backend Locally

Clone the repository:

```bash
git clone https://github.com/Sanjanabandari/smart-campus-bus-backend.git
```

Enter the project directory:

```bash
cd smart-campus-bus-backend
```

On Windows, run the application using the Maven Wrapper:

```powershell
.\mvnw.cmd spring-boot:run
```

The backend uses port `8080` by default, unless configured otherwise.

## API Modules

The application supports these modules:

- Buses
- Routes
- Drivers
- Students
- Schedules

Each module supports CRUD operations through the REST API.

## Frontend Repository

https://github.com/Sanjanabandari/smart-campus-bus-frontend

## Backend Repository

https://github.com/Sanjanabandari/smart-campus-bus-backend

## Project Status

The backend has been tested locally with the React frontend and MySQL database. Online deployment is pending.
