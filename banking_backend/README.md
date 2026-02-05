# 🔐 Banking Backend

Spring Boot based REST API for the Bank Management System.  
Handles authentication, account operations, transactions, and data persistence.

## Features

- RESTful API for account, transaction, and user management
- User authentication and registration
- Email verification
- Transaction and payment history

## ⚙️ Technologies Used

- Java
- Spring Boot
- JWT Authentication
- Maven
- JPA
- MySQL

## Running Backend

### 🗄️ Database Configuration

Update `application.properties`:

```bash
properties
spring.datasource.username=your_username
spring.datasource.password=your_password

```

### 🔐 JWT Configuration

```bash
jwt.app.secret= your_secret_key
```

1. Navigate to this directory:
   ```bash
   cd banking_backend
   ```
2. Build and run the application:
   ```bash
   ./mvnw spring-boot:run
   ```
3. The backend will be run at [http://localhost:8080](http://localhost:8080)

## 🔗 API Endpoints Overview

The backend exposes RESTful APIs secured using JWT authentication.

### 🔐 Authentication & User Management

- **POST** `/register` – Register a new user
- **POST** `/login` – Authenticate user and issue JWT
- **GET** `/verify` – Verify user account via email token

---

### 🏦 Account Management

- **POST** `/account/create_account` – Create a new bank account
- **GET** `/app/dashboard` – Fetch user dashboard details

---

### 💸 Transactions

- **POST** `/transact/deposit` – Deposit funds
- **POST** `/transact/withdraw` – Withdraw funds
- **POST** `/transact/transfer` – Transfer funds to another account

---

### 💳 Payments & History

- **POST** `/transact/payment` – Make a payment
- **GET** `/app/payment_history` – View payment history
- **GET** `/app/transaction_history` – View transaction history

## 📂 Project Structure

```
banking_backend
├── src/main/java/com/bankingApp
│ ├── controllers
│ ├── models
│ ├── repository
│ ├── config
│ ├── helpers
│ └── exception
├── src/main/resources
│ └── application.properties
├── pom.xml
└── README.md
```
