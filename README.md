🚀 A RESTful backend for an e-commerce platform built with Spring Boot, PostgreSQL, and Spring Data JPA, supporting product management with image uploads.

Features
✔ Product Management – CRUD operations for products (Create, Read, Update, Delete).
✔ Image Handling – Upload and retrieve product images stored in the database.
✔ RESTful APIs – Well-structured endpoints for frontend integration.
✔ Database Integration – PostgreSQL with Spring Data JPA for efficient data persistence.
✔ CORS Support – Enabled for seamless frontend-backend communication.
✔ Error Handling – Proper HTTP responses and exception management.

Tech Stack
Backend: Java 21, Spring Boot 3.5.3

Database: PostgreSQL

ORM: Spring Data JPA (Hibernate)

Build Tool: Maven

Libraries: Lombok (for boilerplate reduction)

API Endpoints
Endpoint	Method	Description
/api/products	GET	Get all products
/api/product/{id}	GET	Get a product by ID
/api/product	POST	Add a new product (with image upload)
/api/product/{id}/image	GET	Retrieve a product's image
/healthCheck	GET	Check if the backend is running
Setup & Run
Prerequisites
Java 21

PostgreSQL (update application.properties with your DB credentials)

Maven

Steps
Clone the repo:

sh
git clone https://github.com/your-username/ecom-springboot.git
Configure PostgreSQL in src/main/resources/application.properties:

properties
spring.datasource.url=jdbc:postgresql://localhost:5432/ECOM  
spring.datasource.username=your_username  
spring.datasource.password=your_password  
Build and run:

sh
mvn spring-boot:run
Access APIs at:

text
http://localhost:8080/api/products
Future Improvements
🔹 Add JWT Authentication for secure APIs.
🔹 Implement pagination & filtering for product listings.
🔹 Integrate Swagger/OpenAPI for API documentation.
🔹 Extend with order & user management.
