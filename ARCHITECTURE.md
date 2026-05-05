# Architecture Overview

```
+------------------+
|      Client       |
+------------------+
        |  ^
        |  |
        v  |
+------------------+   +---------------------+
|  REST API Layer  |<->|  Service Layer      |
+------------------+   +---------------------+
        |  ^
        |  |
        v  |
+------------------+   +---------------------+
| Data Access Layer |<->|  PostgreSQL DB     |
+------------------+   +---------------------+
```

## Layer Descriptions
- **Client:** Utilizes RESTful API endpoints.
- **REST API Layer:** Handles incoming requests and sends responses.
- **Service Layer:** Contains business logic and interacts with data access layer.
- **Data Access Layer:** Communicates with PostgreSQL database using Spring Data JPA.

## Data Flow Explanation
1. Client sends an API request.
2. Request is processed by the REST API Layer.
3. Business logic is executed in the Service Layer.
4. Interactions with the database occur through the Data Access Layer.
5. Responses are sent back through the REST API Layer to the Client.

## Key Architecture Decisions
- **Spring Boot:** Chosen for rapid application development.
- **PostgreSQL:** Selected for its robustness and advanced features.
- **JWT Authentication:** Opted for security and scalability in API access.