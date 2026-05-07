# Data Sync Engine

A professional Spring Boot backend designed for enterprise-grade data synchronization workflows.

## Project Overview

This backend provides:

- REST APIs for triggering and retrieving sync job status
- Service layer implementing business orchestration
- Repository layer backed by JPA for persistence
- Scheduled jobs for automated sync operations
- Global exception handling and API error responses
- Structured configuration using placeholders for safe deployment
- Logging utilities for consistent diagnostic output

## Project Structure

- `src/main/java/com/example/datasyncengine`
  - `controller` - REST endpoints
  - `service` - business logic
  - `repository` - data persistence
  - `dto` - request / response models
  - `entity` - JPA entities
  - `config` - configuration and scheduling
  - `exception` - centralized error handling
  - `scheduler` - scheduled job processing
  - `util` - shared utilities

## Getting Started

1. Configure the placeholders in `src/main/resources/application.yml`.
2. Build the project:

```bash
mvn clean package
```

3. Run the application:

```bash
mvn spring-boot:run
```

## Configuration Placeholders

- `DATABASE_URL_PLACEHOLDER`
- `DB_USERNAME_PLACEHOLDER`
- `DB_PASSWORD_PLACEHOLDER`
- `YOUR_API_KEY`
- `JWT_SECRET_PLACEHOLDER`

## API Endpoints

- `POST /api/v1/sync/jobs` - create and execute a sync job
- `GET /api/v1/sync/jobs/{id}` - retrieve job details by ID

## Notes

This project includes placeholder values only and does not contain any sensitive secrets, tokens, or connection strings.
