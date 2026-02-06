# 📚 Book Store Management System

A simple **Spring Boot MVC web application** for managing books using **Spring Boot, Spring Data JPA, Thymeleaf, MySQL, and Bootstrap**.

This project allows users to:
- Add new books
- View all available books
- Edit and delete books
- Add books to a personal “My Book List”
- Remove books from “My Book List”

---
## 🛠️ Screenshots
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1bd18c6e-89b5-4b63-a11b-26e2a19227c5" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/3f0c667f-0e86-4e75-8588-9cde757296cd" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7997cc78-1a63-47c6-a6e4-ffd331691e11" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/570fc6b0-95f6-4011-9bef-d2b55a0df26d" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f487c880-9b71-419b-9426-8bd9db7c9380" />

## 🛠️ Technologies Used

- **Java**
- **Spring Boot**
- **Spring MVC**
- **Spring Data JPA**
- **Thymeleaf**
- **MySQL**
- **Hibernate**
- **Bootstrap 5**
- **Font Awesome**

---

## 🏗️ Project Architecture

The project follows a **layered architecture**:

Controller Layer → Service Layer → Repository Layer → Database


### Layers:
- **Controller** – Handles HTTP requests and navigation
- **Service** – Contains business logic
- **Repository** – Interacts with the database using JPA
- **Entity** – Represents database tables
- **View** – Thymeleaf HTML templates

---

## 📂 Project Structure

com.bookStore
│
├── controller
│ ├── BookController.java
│ └── MyBookListController.java
│
├── entity
│ ├── Book.java
│ └── MyBookList.java
│
├── repository
│ ├── BookRepository.java
│ └── MyBookRepository.java
│
├── service
│ ├── BookService.java
│ └── MyBookListService.java
│
├── templates
│ ├── home.html
│ ├── bookRegister.html
│ ├── bookList.html
│ ├── bookEdit.html
│ └── myBooks.html
│
└── application.properties


---

## 📌 Features

### 🔹 Book Management
- Add new books
- View all available books
- Edit book details
- Delete books

### 🔹 My Book List
- Add books to personal list
- View selected books
- Remove books from the list

### 🔹 UI
- Responsive UI using **Bootstrap**
- Icons using **Font Awesome**

---

## 🗄️ Database Configuration

**MySQL Database**

```properties
server.port=1001

spring.datasource.name=book
spring.datasource.url=jdbc:mysql://localhost:3306/book_store
spring.datasource.username=root
spring.datasource.password=pritee@935636
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL57Dialect
⚠️ Make sure MySQL is running and the book_store database exists.

🧩 Entity Description
📘 Book Entity
Represents all available books in the store.

Fields:
id
name
author
price

📗 MyBookList Entity
Represents books added to the user's personal list.

Fields:
id
name
author
price

🌐 Application URLs
URL	Description
/	Home page
/book_register	Register a new book
/available_books	View all books
/my_books	View My Book List
/editBook/{id}	Edit a book
/deleteBook/{id}	Delete a book
/mylist/{id}	Add book to My Book List
/deleteMyList/{id}	Remove book from My Book List

▶️ How to Run the Project
Clone the repository
Open the project in Spring Tool Suite / IntelliJ / Eclipse
Update database credentials in application.properties
Run the application as Spring Boot App
Open browser and visit:
http://localhost:1001

👩‍💻 Author
Pritee Kolsure
Java & Spring Boot Developer

⭐ Conclusion
This project demonstrates:
Spring Boot MVC architecture
CRUD operations using JPA
Thymeleaf integration
Real-time database interaction
Perfect for learning Spring Boot and interview demonstration.

