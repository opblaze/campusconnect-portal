# Campus Connect — Smart Student Portal

Campus Connect is a Java web application for student, faculty, and administrator workflows. It uses Servlets, JSP/JSTL, Spring dependency injection, Hibernate, and MySQL.

## Features

Student and faculty dashboards, attendance, assignments, marks, study material, timetable, exams, fees, announcements, feedback, notifications, search, and a campus-focused chatbot. The project also includes a Swing faculty console and a Progressive Web App interface.

## Source archive

[Download the complete source ZIP](CampusConnect-Source.zip). It contains the project source, SQL schema and synthetic seed data, documentation, and sample checks. Generated Maven `target/` output is excluded. Seeded names and contact fields are anonymized; `.invalid` email addresses are placeholders.

## Run locally

1. Install Docker Desktop.
2. Download and extract the source ZIP.
3. From the extracted project folder, run `docker compose up --build`.
4. Open `http://localhost:8080`.

The Docker image uses Tomcat 11 and Java 21; the database uses MySQL 8.4. The chatbot falls back to local answers when no Gemini API key is configured. Email integration is optional. See `docs/DEPLOYMENT.md` inside the ZIP for configuration details.

## Demo accounts

| Role | Login | Password |
|---|---|---|
| Student | `DEMO-STU-001` | `Student@123` |
| Student | `DEMO-STU-002` | `Student@123` |
| Student | `DEMO-STU-003` | `Student@123` |
| Faculty | `DEMO-FAC-001` | `Faculty@123` |
| Faculty | `DEMO-FAC-002`–`DEMO-FAC-006` | `Faculty@123` |
| Admin | `admin@example.invalid` | `Admin@123` |

These are public demo credentials for the synthetic local dataset only. Do not reuse them for real accounts.

## Deployment

The source repository is public. The live application deployment is on hold, so there is no public runtime link yet. The app requires a Docker-capable Java host and a MySQL database.
