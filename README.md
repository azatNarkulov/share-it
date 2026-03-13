# Share It

Backend service for sharing items between users.
The platform allows users to lend items to others, request bookings, and manage availability.

The project demonstrates building a RESTful backend application with business logic for item sharing and booking management.

---

## Features

* Add and manage items available for sharing
* Search items by text query
* Create and manage booking requests
* Approval or rejection of booking requests by item owners
* Leave comments after completed bookings
* User and item management

---

## Architecture

The application follows a layered backend architecture:

* **Controller layer** — REST API endpoints
* **Service layer** — business logic
* **Repository layer** — database interaction

Requests are processed through REST controllers and persisted in the database using JPA/Hibernate.

---

## Tech Stack

**Backend**

* Java
* Spring Boot
* REST API
* Maven

**Persistence**

* PostgreSQL
* H2 (for testing)
* JPA / Hibernate

**Other**

* Lombok
* MapStruct
* Docker
* Postman (API testing)

---

## API

The service exposes several groups of REST endpoints:

* **Users** — user management
* **Items** — item creation, updates, and search
* **Bookings** — booking requests and approval workflow
* **Comments** — feedback for completed bookings

API requests and examples can be tested using the Postman collection included in the repository.

---

## Running the project

### Requirements

* Java 21
* Maven
* Docker (optional)

### Run with Docker

```bash
docker-compose up
```

### Run locally

```bash
mvn clean package
mvn spring-boot:run
```

---

## Project Structure

```
gateway    — API gateway for request validation and routing
server     — main service with business logic
postman    — API testing collection
```

---

## Key Backend Concepts

This project demonstrates:

* REST API design
* layered architecture
* database modeling and relationships
* request validation
* booking workflow implementation
