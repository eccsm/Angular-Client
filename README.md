# Angular Client with Spring REST Backend

This project is an Angular client application that interacts with a Spring RESTful backend server. It demonstrates a full-stack web application with a focus on frontend development using Angular and backend services provided by Spring Boot.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Configuration](#configuration)
  - [Running the Application](#running-the-application)
- [Folder Structure](#folder-structure)
- [Contributing](#contributing)
- [License](#license)

## Features

- Integration between Angular frontend and Spring RESTful backend
- Demonstrates CRUD operations
- Organized project structure for scalability
- Example of service consumption in Angular

## Technologies Used

- [Angular](https://angular.io/) for the frontend
- [Spring Boot](https://spring.io/projects/spring-boot) for the backend
- [Node.js](https://nodejs.org/) as the runtime environment for Angular
- [TypeScript](https://www.typescriptlang.org/) for client-side scripting
- [Java](https://www.java.com/) for server-side development

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) installed on your machine
- [Angular CLI](https://angular.io/cli) installed globally
- [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) installed
- [Spring Boot](https://spring.io/projects/spring-boot) set up for the backend server
- [Git](https://git-scm.com/) for version control

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/eccsm/Angular-Client.git
   cd Angular-Client
   ```

2. **Install Angular client dependencies:**
   ```bash
   npm install
   ```

3. **Set up the Spring Boot backend:**
   - Ensure you have the backend server running. If it's a separate project, follow its setup instructions to start the server.

### Configuration

1. **Angular Environment Configuration:**
   - Navigate to the `src/environments` directory.
   - Update the `environment.ts` and `environment.prod.ts` files to match your API backend configuration.
   - Example:
     ```typescript
     export const environment = {
       production: false,
       apiUrl: 'http://localhost:8080/api'
     };
     ```

### Running the Application

1. **Start the Angular Client:**
   ```bash
   ng serve
   ```
   - The Angular application will start on `http://localhost:4200/` by default.

2. **Start the Spring Boot Backend:**
   - If using a separate backend, ensure it's running on `http://localhost:8080/` or the configured API URL.

## Folder Structure

```
Angular-Client/
├── src/
│   ├── app/
│   ├── assets/
│   ├── environments/
│   ├── index.html
│   ├── main.ts
│   ├── styles.scss
│   ├── angular.json
│   ├── package.json
│   ├── README.md
└── backend/
    ├── src/
    ├── main/
    ├── java/
    ├── com/
    ├── config/
    ├── controllers/
    ├── models/
    ├── services/
    ├── application.properties
    ├── pom.xml
    ├── README.md
```

- `src/`: Contains the Angular front-end application.
  - `app/`: Source code for the Angular app.
  - `environments/`: Configuration files for API endpoints.
  - `styles.scss`: Global styles for the app.
  - `package.json`: Lists client-side dependencies and scripts.
- `backend/`: Contains the Spring Boot back-end application.
  - `controllers/`: Defines RESTful API endpoints.
  - `models/`: Data models for handling application data.
  - `services/`: Business logic for handling requests.
  - `application.properties`: Backend configuration.
  - `pom.xml`: Maven build configuration.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any enhancements, bug fixes, or suggestions.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
