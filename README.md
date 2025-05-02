# ✈️ Airline Management System

This project is an Airline Management System developed using **Java Spring Boot** for the backend and **Angular (v12.1.1)** with **TypeScript** for the frontend.

It provides an intuitive platform for both administrators and users to manage flight reservations, flight schedules, and user information efficiently.

## 🔧 Technologies Used

### Backend:
- Java
- Spring Boot
- SOLID Principles
- MVC Architecture
- DAO Design Pattern (with DAO, DAOImpl, Entity, Controller, Service, Helper layers)
- RowMapper for database mapping
- MySQL

### Frontend:
- Angular 12.1.1
- TypeScript
- HTML/CSS
- Bootstrap


## 🔐 Roles & Features

### ✈️ Admin:
- Secure login
- Add new flight details (including flight duration)
- View number of reservations per flight
- Manage flight data

### 👤 User:
- Sign up and sign in functionality
- Make a reservation
- View total price of the booking
- Cancel reservations
- Edit personal information

## 📁 Backend Structure

- `controller/` – Handles HTTP requests.
- `service/` – Contains business logic.
- `entity/` – Contains model classes.
- `dao/` – Interface for data access.
- `daoImpl/` – Implements DAO with SQL logic.
- `helper/` – Contains utility and RowMapper classes for database mapping.

## 🚀 Running the Angular Frontend

### Prerequisites
- Node.js (v14 or above)
- Angular CLI installed globally:

  bash
  npm install -g @angular/cli


## 🖥️ Backend Setup – Spring Boot (Java)

This is the backend for the Airline Management System developed using **Java Spring Boot**. The backend follows **SOLID principles** and the **MVC architecture**, ensuring maintainability and scalability.

---

### 🧱 Project Structure
src/
├── controller/ # Handles API requests and routing
├── service/ # Contains business logic
├── entity/ # Java models mapped to database tables
├── dao/ # DAO interfaces for database operations
├── daoImpl/ # Implements the DAO interfaces
├── helper/ # Utility classes like RowMapper
├── application.properties
└── AirlineManagementSystemApplication.java

### 💡 Key Features

- Clean and modular code with well-separated layers (Controller, Service, DAO)
- Uses RowMapper for mapping SQL results to objects
- Follows SOLID principles for clean architecture
- Secure login and role-based access for admin and users
- Handles user registration, login, reservations, cancellations, and profile edits
- Admin can manage flights and view reservations

### 🛠 Prerequisites

- Java 8 or higher
- Spring Tool Suite (STS) IDE
- MySQL (or compatible DB)
- Maven (for dependency management)

### 🔧 Configuration

1. **Database Configuration:**

Update your `src/main/resources/application.properties` with your DB config:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/airline_db
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true


▶️ Running the Project
Open Spring Tool Suite (STS).

Click on File > Import > Existing Maven Projects.

Navigate to the project directory and select it.

Let STS download the dependencies.

Right-click on the main class (AirlineManagementSystemApplication.java) and select Run As > Spring Boot App.

The server should start on http://localhost:8080.

🧪 Testing
Use Postman or the Angular frontend to test all endpoints.

Handle validation and exceptions with appropriate HTTP status codes.

🚨 Notes
Enable CORS for frontend integration:

@CrossOrigin(origins = "http://localhost:4200")
Use BCrypt for password encryption (optional but recommended).

📫 Contact
For backend issues, bugs, or suggestions, feel free to open an issue in the repository.

