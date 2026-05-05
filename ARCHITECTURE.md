# Architecture Overview

## ASCII Diagrams
```
   +---------------+       +-----------------+
   |   Controller  |<----->|   Service Layer  |
   +---------------+       +-----------------+
            |                          |
            |                          |
            v                          v  
   +---------------+       +-----------------+
   |    Model      |<----->|   Repository     |
   +---------------+       +-----------------+
```

## Layer Descriptions and Responsibilities
- **Controller Layer:** Handles incoming API requests and maps them to the appropriate service methods.
- **Service Layer:** Contains business logic and serves as a bridge between the controller and repository.
- **Model Layer:** Defines the data structures used throughout the application.
- **Repository Layer:** Responsible for data access and management, interacting with the PostgreSQL database.

## Data Flow Explanation
1. A client sends an HTTP request to the controller.
2. The controller processes the request and calls the corresponding service method.
3. The service layer performs business logic, potentially calling repository methods to access or persist data.
4. The repository interacts with the PostgreSQL database to fulfill the data request.
5. The response flows back up to the client through the service and controller layers.

## Key Architecture Decisions
- **Spring Boot Framework:** Chosen for its simplicity and ease of use in building REST APIs.
- **PostgreSQL:** Selected for its robustness and support for complex queries and transactions.
- **JWT for Authentication:** Provides a stateless and scalable method for securing endpoints.