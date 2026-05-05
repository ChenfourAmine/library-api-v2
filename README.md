# Library API

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Java](https://img.shields.io/badge/java-17-brightgreen.svg)

## Description

A simple REST API for managing a library system that includes books and authors. This project leverages Spring Boot, PostgreSQL, and JWT for authentication.

## Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/ChenfourAmine/library-api-v2.git
   cd library-api-v2
   ```

2. Ensure you have Java 17 and Maven installed.

3. Install PostgreSQL and create a database for the application.

4. Update `application.properties` file with your database configuration.

5. Run the application:
   ```bash
   mvn spring-boot:run
   ```

## Usage Example

- To create a new book:
   ```bash
   POST /api/books
   {
       "title": "The Great Gatsby",
       "authorId": 1
   }
   ```

- To retrieve all books:
   ```bash
   GET /api/books
   ```

## Contributing

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to the Spring Boot community.

---

## Best Practices
- Use Spring Boot starters for quick dependency management.
- Implement RESTful principles for designing your API.
- Follow the MVC architecture for separation of concerns.
- Use DTOs (Data Transfer Objects) to decouple your API from the internal models.
- Utilize Spring Data JPA for interacting with PostgreSQL.