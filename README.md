# 💰 Money Manager Application - Backend

Welcome to the backend repository of the **Money Manager Application**. This application is built with **Spring Boot** and serves as the robust foundation for managing finances, offering authorized APIs for transaction tracking, category management, and visual analytics.

## 🚀 Key Features

- **Secure Authentication**: JWT-based security system.
- **Transaction Management**: APIs for income and expense tracking.
- **Category Customization**: Manage financial categories dynamically.
- **Visual Analytics Data**: Endpoints to serving data for charts and trends.
- **Reporting**: Financial overview and smart filtering capabilities.

## 🛠 Tech Stack

- **Framework**: Spring Boot
- **Database**: MySQL
- **Security**: Spring Security with JWT
- **ORM**: Spring Data JPA
- **Build Tool**: Maven

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- **Java 17** (or higher)
- **MySQL Server**
- **Postman** (for API testing)

## ⚙️ Configuration

### 1. Database Setup
Create a MySQL database named `moneymanager`.
```sql
CREATE DATABASE moneymanager;
```

### 2. Application Properties
Navigate to `src/main/resources/application.properties` and configure your database credentials.

**Important:** By default, the application might have `spring.profiles.active=prod` enabled, which points to a remote PostgreSQL database. To run locally with MySQL:
1. Open `src/main/resources/application.properties`.
2. **Comment out** the line `spring.profiles.active=prod` to use the default MySQL configuration.
3. Update the username and password if they differ from your local MySQL setup:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/moneymanager
spring.datasource.username=YOUR_MYSQL_USERNAME
spring.datasource.password=YOUR_MYSQL_PASSWORD
```

### 3. Environment Variables
The application requires the following environment variables for email features and frontend integration. You can set them in your IDE or system environment, or replace them manually in `application.properties`:

- `MAIL_USERNAME` (SMTP email)
- `MAIL_PASSWORD` (SMTP password)
- `MAIL_FROM` (Sender email address)
- `MONEY_MANAGER_FRONTEND_URL` (e.g., `http://localhost:3000`)
- `MONEY_MANAGER_BACKEND_URL` (e.g., `http://localhost:8080/api/v1.0`)

## 🏃‍♂️ How to Run

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd moneymanagerbackend
   ```

2. **Build the application**:
   ```bash
   ./mvnw clean install
   ```
   *(On Windows, use `mvnw cmd clean install` or just `mvnw clean install`)*

3. **Run the application**:
   ```bash
   ./mvnw spring-boot:run
   ```

The backend server will start at `http://localhost:8080`.

## 🔌 API Documentation

The base URL for all API endpoints is:
`http://localhost:8080/api/v1.0`

**Common Endpoints:**
- `POST /api/v1.0/auth/login` - User Login
- `POST /api/v1.0/auth/register` - User Registration
- `GET /api/v1.0/transactions` - Get All Transactions

(Use **Postman** to import and test the collection of API requests).
