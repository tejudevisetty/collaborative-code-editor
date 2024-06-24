
# Collaborative Code Editor Tool

## Overview

The Collaborative Code Editor Tool is a web-based application that allows multiple users to collaboratively edit and manage documents in real-time. Built with Spring Boot, WebSocket, and H2 Database, this tool ensures a seamless and synchronized editing experience.

## Features

- **Real-time Collaboration**: Multiple users can edit documents simultaneously.
- **Document Management**: Create, read, update, and delete documents.
- **User Authentication**: Secure login and user management.
- **WebSocket Communication**: Real-time updates using WebSocket.
- **In-memory Database**: H2 Database for easy setup and testing.
- **RESTful APIs**: Endpoints for managing documents and users.


## Getting Started

### Prerequisites

- Java 11 or higher
- Maven
- An IDE (e.g., Eclipse, IntelliJ IDEA)

### Installation

1. **Clone the repository:**

   ```sh
   git clone https://github.com/tejudevisetty/collaborative-code-editor.git
   cd CollaborativeCodeEditorTool
   ```

2. **Build the project:**

   ```sh
   mvn clean install
   ```

3. **Run the application:**

   ```sh
   mvn spring-boot:run
   ```

### Configuration

The application is configured using the `application.properties` file located in the `src/main/resources` directory. Here are some key configurations:

```properties
# Server Configuration
server.port=8081

# H2 Database Configuration
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=teju
spring.datasource.password=teju@123
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.h2.console.enabled=true
spring.h2.console.path=/h2-console

# JPA Configuration
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

# Logging Configuration (optional)
logging.level.org.springframework=INFO
logging.level.com.example=DEBUG

spring.devtools.livereload.enabled=true
spring.devtools.livereload.port=35730


## Testing the APIs

Use Postman or a similar tool to test the RESTful APIs.

## Running Tests

To run the tests, use the following command:

```sh
mvn test
```

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for review.

## License

This project is licensed under the MIT License.

