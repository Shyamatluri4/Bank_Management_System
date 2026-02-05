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


### ❗ Common Issues

-400 / 500 errors → Check request body & validation
-JWT errors → Verify secret key consistency


## 📂 Project Structure

`
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
`
