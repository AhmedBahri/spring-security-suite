# Spring Security Suite

A comprehensive Spring Boot application that showcases various Spring Security features, including OAuth2, JWT, LDAP, and form-based authentication. This project aims to provide a foundational structure for developers looking to implement robust security mechanisms in their Spring applications.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Technologies Used](#technologies-used)
3. [Features](#features)
4. [Prerequisites](#prerequisites)
5. [Getting Started](#getting-started)
6. [Configuration](#configuration)
7. [Usage](#usage)
8. [Testing](#testing)
9. [Contributing](#contributing)
10. [License](#license)

## Project Overview

The Spring Security Suite is designed to demonstrate the implementation of various security features in a Spring Boot application. It serves as a reference for developers who want to understand and implement advanced security mechanisms in their own projects.

## Technologies Used

- Java 17
- Spring Boot 3.3.3
- Spring Security
- Spring Data JPA
- Spring Data LDAP
- Spring OAuth2
- Thymeleaf
- PostgreSQL
- Lombok
- Okta Spring Boot Starter
- Maven

## Features

1. **OAuth2 Integration**:
    - Authorization Server
    - Resource Server
    - Client

2. **LDAP Authentication**: Lightweight Directory Access Protocol for user authentication.

3. **JWT (JSON Web Token)**: Secure information transmission between parties.

4. **Form-based Authentication**: Traditional username/password authentication.

5. **Database Integration**: Using PostgreSQL for data persistence.

6. **Thymeleaf Templates**: Server-side Java template engine for web views.

7. **Session Management**: Using Spring Session for session handling.

8. **Okta Integration**: Additional authentication and authorization options.

## Prerequisites

- JDK 17
- Maven 3.x
- PostgreSQL database
- (Optional) LDAP server for LDAP authentication

## Getting Started

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/spring-security-suite.git
   ```

2. Navigate to the project directory:
   ```
   cd spring-security-suite
   ```

3. Build the project:
   ```
   mvn clean install
   ```

4. Run the application:
   ```
   mvn spring-boot:run
   ```

## Configuration

1. Database Configuration:
    - Update `src/main/resources/application.properties` with your PostgreSQL credentials.

2. LDAP Configuration (if using):
    - Configure LDAP properties in `application.properties`.

3. OAuth2 Configuration:
    - Set up OAuth2 client credentials and endpoints in `application.properties`.

4. Okta Configuration:
    - Add Okta properties to `application.properties` as per your Okta application settings.

## Usage

After starting the application, you can access different endpoints to test various security features:

- `/`: Home page
- `/login`: Login page for form-based authentication
- `/oauth2/authorization/client-id`: OAuth2 login
- `/api/secured`: A secured API endpoint (requires authentication)

Refer to the controller classes for more specific endpoints and their security configurations.

## Testing

Run the tests using:

```
mvn test
```

The project includes both unit and integration tests to ensure the security features are working as expected.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

[Your chosen license]

---

For more information on Spring Security, please refer to the [official Spring Security documentation](https://docs.spring.io/spring-security/reference/index.html).
