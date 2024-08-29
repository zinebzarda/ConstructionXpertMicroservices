# ConstructionXpert Services - Project Management Application

## Description
This project is a microservices-based application developed for "ConstructionXpert Services" to manage construction projects. The application includes services for managing projects, tasks, and resources, each with its own database to ensure data isolation and ease of maintenance.

## Technologies Used
- **Backend**: Spring Boot, Spring Cloud, Spring Data JPA, Flyway
- **Frontend**: Angular
- **Database**: PostgreSQL/MySQL (separate databases for each microservice)
- **API Communication**: RESTful APIs
- **Version Control**: Git

## Microservices

### 1. Project Management Service
- **Features**:
  - Create a new project with name, description, start date, end date, and budget.
  - View a list of existing projects with details.
  - Update project details.
  - Delete an existing project.

### 2. Task Management Service
- **Features**:
  - Create a new task with description, start date, end date, status (to-do, in progress, completed), and required resources.
  - View a list of tasks associated with a project.
  - Update task details.
  - Delete an existing task.

### 3. Resource Management Service
- **Features**:
  - Add new resources with details such as name, type, quantity, and supplier information.
  - View a list of available resources.
  - Update resource details.
  - Delete an existing resource.

## Database Management
- Each microservice has its own database.
- **Flyway** is used for database schema migrations, ensuring version-controlled and orderly application of schema changes during deployments.

## Setup and Installation

### Prerequisites
- JDK 17+
- PostgreSQL/MySQL

### Installation Steps

1. **Clone the repository**:
    ```bash
    git clone https://github.com/username/constructionxpert-services.git
    cd constructionxpert-services
    ```

3. **Apply database migrations**:
    Each microservice will automatically apply migrations using Flyway upon startup.

4. **Access the services**:
    - Project Management Service: `http://localhost:8081`
    - Task Management Service: `http://localhost:8082`
    - Resource Management Service: `http://localhost:8083`
    - eurika: 'http://localhost:8761/eureka/'

## Usage
- Use the provided RESTful APIs to interact with the services.
- Access the frontend to manage projects, tasks, and resources through a user-friendly interface.


