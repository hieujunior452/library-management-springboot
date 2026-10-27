# Library Management System

Hệ thống quản lý thư viện xây dựng bằng Spring Boot, MySQL, và JPA.

## Công nghệ

- **Backend:** Java 17, Spring Boot 3.x, Spring Data JPA
- **Database:** MySQL 8
- **Build:** Maven
- **Documentation:** Swagger/OpenAPI (Springdoc)
- **Migration:** Flyway

## Yêu cầu

- JDK 17 hoặc cao hơn
- Maven 3.8+
- MySQL 8 (hoặc Docker)
- Docker Desktop (tùy chọn, để chạy MySQL)

## Cách chạy

### 1. Chạy MySQL bằng Docker

```bash
docker run -d --name library-mysql -p 3306:3306 \
  -e MYSQL_ROOT_PASSWORD=root \
  -e MYSQL_DATABASE=library \
  mysql:8
```

### 2. Clone project và tải dependency

```bash
git clone https://github.com/your-username/library-management-springboot.git
cd library-management-springboot
mvn clean install
```

### 3. Chạy app

```bash
mvn spring-boot:run
```

Hoặc chạy thẳng trong IDE (chọn file `LibraryApplication` → Run).

### 4. Truy cập Swagger UI

Mở trình duyệt:
