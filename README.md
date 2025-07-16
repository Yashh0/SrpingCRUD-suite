# 🧪 SBJunit5 – Spring Boot Project for JUnit5 Testing

A comprehensive Spring Boot application template with integrated JUnit5 testing and MySQL support. This project demonstrates how to build, test, and document RESTful services using the latest Spring Boot stack.

---

## 📦 Features

- ✅ Spring Boot 3.0.4
- ✅ Java 17+
- ✅ RESTful API with Spring Web
- ✅ Data persistence using Spring Data JPA
- ✅ MySQL database with auto DDL
- ✅ Swagger UI for interactive API documentation
- ✅ JUnit 5 for unit and integration testing
- ✅ DevTools for hot reloading
- ✅ Maven build system

---

## ⚙️ Technologies Used

| Tool            | Version  |
|-----------------|----------|
| Spring Boot     | 3.0.4    |
| Java            | 17+      |
| Maven           | Latest   |
| MySQL           | 8+       |
| JUnit           | 5        |
| Swagger (SpringDoc) | 2.0.4 |

---

## 🚀 How to Run

1. **Start MySQL** and ensure the user/password is set as:
   - Username: `root`
   - Password: 

2. **Clone the repo**:

```bash
git clone https://github.com/your-username/SBJunit5.git
cd SBJunit5
```

3. **Run the project**:

```bash
mvn spring-boot:run
```

The app will start at: `http://localhost:8888`

---

## 📊 API Documentation

Visit:
```
http://localhost:8888/swagger-ui.html
```

Explore and test all endpoints from a browser.

---

## 🧪 Running Tests

To run all tests:

```bash
mvn test
```

JUnit 5 tests are located under `src/test/java/...`.

---

## 🛠 Configuration

File: `src/main/resources/application.yml`

```yaml
server:
  port: 8888

spring:
  datasource:
    driver-class-name: com.mysql.cj.jdbc.Driver
    url: jdbc:mysql://localhost:3306/sbjunit5?createDatabaseIfNotExist=true&autoReconnect=true&allowPublicKeyRetrieval=true&useSSL=false
    username: root
    password: root
  jpa:
    hibernate:
      ddl-auto: update
    show-sql: true
    properties:
      hibernate:
        dialect: org.hibernate.dialect.MySQLDialect
```

---

## 📁 Project Structure

```
SBJunit5/
├── src/
│   ├── main/
│   │   ├── java/com/csi/...
│   │   └── resources/
│   │       └── application.yml
│   └── test/java/com/csi/...
├── pom.xml
└── README.md
```

---

## 🤝 Contribution

Pull requests are welcome. For major changes, open an issue first to discuss what you would like to change.

---

