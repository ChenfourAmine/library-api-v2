# Library API

![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen.svg)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-13.x-blue.svg)
![Maven](https://img.shields.io/badge/Maven-3.x-orange.svg)

## Description
Library API is a simple REST API for managing a library system with books and authors.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/ChenfourAmine/library-api-v2.git
   cd library-api-v2
   ```
2. Configure your PostgreSQL database in `application.properties`.
3. Build the project using Maven:
   ```bash
   mvn clean install
   ```
4. Run the application:
   ```bash
   mvn spring-boot:run
   ```

## Usage
- Base URL: `http://localhost:8080/api`
- Authentication: Use JWT tokens for secure access.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.

## License
This project is licensed under the MIT License.