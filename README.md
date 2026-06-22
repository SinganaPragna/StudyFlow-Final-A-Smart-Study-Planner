# StudyFlow – Smart Study Planner

## Overview

StudyFlow is a web application developed to help students effectively organize, plan, and manage their academic activities. The platform provides an intuitive interface for managing subjects, scheduling study sessions, maintaining personal study notes, and tracking learning progress in one centralized system.

The application is designed to improve productivity and time management by enabling students to create structured study plans, monitor completed tasks, and maintain organized academic records. By integrating a React-based frontend, a Spring Boot backend, and a MySQL database, StudyFlow delivers a seamless and efficient study management experience.

## Features

- User Registration and Login
- Subject Management
- Study Session Planning
- Time Table Generation
- Notes Management
- Progress Tracking
- Clear Dashboard
- Responsive User Interface

## Tech Stack

### Frontend
- React
- Vite
- TypeScript
- Tailwind CSS

### Backend
- Java
- Spring Boot
- REST API

### Database
- MySQL

## Project Architecture

Frontend (React + Vite)
↓
REST API
↓
Spring Boot Backend
↓
MySQL Database

## Local Setup

### Prerequisites

* Java 17 or later
* Apache Maven
* MySQL Server
* Node.js and npm

### Database Setup

1. Start MySQL Server.
2. Create a database named:

```sql
CREATE DATABASE studyplanner;
```

3. Configure database settings in:

```text
java-backend/src/main/resources/application.properties
```

Example:

```properties
spring.datasource.url=jdbc:mysql://localhost:3308/studyplanner?useSSL=false&allowPublicKeyRetrieval=true&serverTimezone=UTC
spring.datasource.username=root
spring.datasource.password=your_mysql_password
```

### Run Backend

Open a terminal in:

```text
java-backend
```

Run:

```bash
mvn spring-boot:run
```

Backend URL:

```text
http://localhost:8090/api
```

### Run Frontend

Open another terminal in:

```text
artifacts/study-planner
```

Install dependencies:

```bash
npm install
```

Run the frontend:

```bash
npm run dev
```

Frontend URL:

```text
http://localhost:5173
```

## Project Structure

```text
Study-Wise-Planner/
│
├── artifacts/study-planner/      # React Frontend
├── java-backend/                 # Spring Boot Backend
├── screenshots/                  # Project Screenshots
└── README.md
```

## Future Enhancements

* Email Notifications
* Task Reminders
* Cloud Deployment
