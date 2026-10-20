# SmartAcademicFlow

**SmartAcademicFlow** is an intelligent academic management platform designed to streamline and automate academic processes in higher education institutions. It centralizes grade management, academic deliberations, make-up exams, and student tracking while integrating AI-powered tools to support academic decision-making.

## Overview

Academic management often involves complex workflows, repetitive administrative tasks, and coordination between multiple stakeholders. SmartAcademicFlow addresses these challenges through a centralized platform that improves data consistency, simplifies academic operations, and facilitates access to academic information.

The platform provides dedicated workspaces for teachers, module coordinators, program directors, and academic administration.

## Key Features

- **Grade Management:** Enter, update, and track student grades.
- **Academic Deliberations:** Review module results and support academic decision-making.
- **AI-Assisted Recommendations:** Analyze borderline cases and provide recommendations for grade adjustments.
- **Make-up Exam Management:** Track make-up sessions and calculate final module results.
- **Teacher Follow-ups:** Monitor grade submission progress and send reminders to teachers.
- **Absence Management:** Record student absences and process supporting documents.
- **AI-Powered Document Analysis:** Extract relevant information from medical certificates using OCR.
- **Academic Regulation Assistant:** Query academic regulations through a Retrieval-Augmented Generation (RAG) system.
- **Academic Reporting:** Consolidate results and export grade data in CSV format for integration with Apogée.
- **Security and Traceability:** Role-based access control, JWT authentication, and audit logs.

## Architecture

SmartAcademicFlow follows a microservices-based architecture composed of five main services:

| Component | Technology | Responsibility |
|---|---|---|
| Frontend | Next.js, React, TypeScript | User interface |
| Backend | Java, Spring Boot | Business logic and REST APIs |
| AI Service | Python, FastAPI | AI assistance, RAG, and OCR |
| Database | PostgreSQL | Persistent data storage |
| Cache | Redis | Caching and session-related operations |

The services communicate through REST APIs and internal HTTP requests. Docker Compose is used to orchestrate the application services.


<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/29eccb7e-e92a-46dc-93de-4d076bf9435e" />


##  Technology Stack

### Frontend
- Next.js
- React
- TypeScript
- Tailwind CSS

### Backend
- Java 21
- Spring Boot
- Spring Security
- Spring Data JPA / Hibernate
- JWT authentication

### Artificial Intelligence
- Python
- FastAPI
- Retrieval-Augmented Generation (RAG)
- Tesseract OCR
- Text and document processing

### Data and Infrastructure
- PostgreSQL
- Redis
- Docker
- Docker Compose

### Development Tools
- Git and GitHub
- Visual Studio Code
- IntelliJ IDEA
- Postman
- Draw.io

## User Roles

The platform supports four main operational roles:

| Role | Responsibilities |
|---|---|
| **Teacher (ENS)** | Enter grades, declare absences, and consult reminders and grade history. |
| **Module Coordinator (RM)** | Monitor grade submissions, send reminders, validate results, and manage deliberations. |
| **Program Director (CF)** | Supervise modules, consolidate semester results, and validate semester reports. |
| **Academic Administration (SCO)** | Manage absences and supporting documents, review results, and export academic data. |

##  Security

Security mechanisms include:

- JWT-based authentication.
- Role-Based Access Control (RBAC).
- Password hashing with BCrypt.
- Protected REST endpoints.
- Audit logging for traceability of academic operations.

##  Getting Started

### Prerequisites

Make sure the following tools are installed:

- Git
- Docker
- Docker Compose

If you intend to run the services outside Docker, you will also need the relevant runtimes and dependencies for Java, Node.js, and Python.

### Installation

Clone the repository:

```bash
git clone https://github.com/OuidadELBJ/Smart-Academic-Flow.git
cd Smart-Academic-Flow
```

### Configuration

Before starting the application, configure the environment variables required by the services.

Use the project's environment configuration files or examples, if available. Do not commit secrets, passwords, API keys, or production credentials to GitHub.

### Run with Docker Compose

If the repository contains a configured `docker-compose.yml` file, start the services with:

```bash
docker compose up --build
```

To stop the services:

```bash
docker compose down
```

**Note:** The exact startup procedure may depend on the environment variables and configuration files provided by the project.

##  Project Structure

The application is organized around three main application layers and supporting infrastructure:

```text
Smart-Academic-Flow/
├── frontend/       # Next.js web application
├── backend/        # Spring Boot REST API
├── ai-service/     # FastAPI AI service
├── docker-compose.yml
└── README.md
```

*The directory names above are illustrative; adapt them to match the actual repository structure.*

##  Project Objectives

- Centralize academic information and workflows.
- Reduce repetitive administrative tasks.
- Improve the reliability and traceability of academic operations.
- Assist academic staff with AI-powered analysis and recommendations.
- Simplify the management of grades, deliberations, and make-up exams.
- Facilitate the exchange of academic data with existing systems.

##  Authors

- **Ouidad EL BOJADDAINI**
- **Ikram MOULAY**

**Academic Supervisor:** Prof. Bouchra BERRADA

**Institution:** National School of Computer Science and Systems Analysis (ENSIAS), Rabat, Morocco

**Academic Year:** 2025–2026

You can check the report for more details <3
