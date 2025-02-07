# SmartRouteX - Mircoservices Design and Development

> [!NOTE]
> The project is part of the "Microservice Design and Development" course and is intended solely for the final project submission.

## Prerequisites

Ensure you have the following installed:

- **Java 17+** (Check with `java -version`)
- **Maven 3+** (Check with `mvn -version`)
- **IDE** (IntelliJ IDEA, Eclipse, or VS Code)

## Setup Instructions

### 1. Clone the Repository
```sh
git clone https://github.com/your-username/routex.git
cd routex
```

### 2. Build the Project
Run the following command to download dependencies and compile the project:

```sh
mvn clean install
```

### 3. Run the Application
You can start the Spring Boot application using:

```sh
mvn spring-boot:run
```

Or run it from your IDE by executing `RoutexApplication.java`.

### 4. Test the API
Once the application is running, open your browser or use **cURL/Postman** to test:

```
GET http://localhost:8080/api/hello
```

Expected response:
```json
{"message":"Healty"}
```

## Project Structure
```
/routex
│-- src/main/java/net/peeranat/routex
│   ├── RoutexApplication.java  # Main entry point
│   ├── controller
│   │   ├── RoutexController.java  # REST API controller
│-- pom.xml  # Maven dependencies
│-- README.md  # Project setup guide
```

## Dependencies Used
- **Spring Boot Starter Web** (For REST API)
- **Maven** (For build management)

## Additional Notes
- The default port is `8080`. Change it in `application.properties` if needed:

  ```properties
  server.port=8081
  ```

- To package the application into a JAR file:

  ```sh
  mvn clean package
  ```

- Run the JAR file:

  ```sh
  java -jar target/routex-0.0.1-SNAPSHOT.jar
  ```

## License
This project is licensed under the **MIT License**.
