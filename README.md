
# 📚 Library Management System - Backend (Hibernate + Java)

This is a **Library Management System** backend developed using **Core Java**, **Hibernate (ORM)**, and **MySQL**. It allows for basic library operations such as managing books and users, issuing and returning books, and maintaining records.

---

## 🚀 Features

- Add, update, delete, and fetch book and user data
- Issue and return books
- Uses Hibernate for database interactions
- Layered architecture (Entity, DAO, Service, Controller)
- Simple and modular Java code structure

---

## 🛠️ Tech Stack

- **Java**
- **Hibernate**
- **MySQL**
- **JDBC**
- **Lombok** (optional)
- **Maven**

---

## 📁 Project Structure

src/
├── main/
│ ├── java/com/example/
│ │ ├── controller/ → Serves as main logic entry point
│ │ ├── service/ → Business logic
│ │ ├── entity/ → POJOs annotated with Hibernate
│ │ ├── daointerface/ → DAO interfaces
│ │ ├── utility/ → Response messages, helper classes
│ │ └── code/ → Hibernate configuration (e.g., SessionFactory)
│ └── resources/ → Hibernate config files (hibernate.cfg.xml, etc.)

yaml
Copy
Edit

---

## ⚙️ How to Run

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/poojabaviskar/Library_Management_System_Backend.git
   cd Library_Management_System_Backend
Set up MySQL Database:

Create a new database in MySQL (e.g., library_db)

Update hibernate.cfg.xml file with:

Database URL

Username and password

Hibernate dialect and driver settings

Compile and Run the Project:

Use an IDE like IntelliJ or Eclipse

Run the main Java file containing main() method or test classes

Make sure the hibernate.cfg.xml is in your classpath (resources folder)

🧪 Sample Functionalities
BookController

addBook()

deleteBook()

updateBook()

getAllBooks()

IssueController

issueBook()

returnBook()

🔑 Configuration
Example hibernate.cfg.xml snippet:

xml
Copy
Edit
<hibernate-configuration>
  <session-factory>
    <property name="hibernate.connection.driver_class">com.mysql.cj.jdbc.Driver</property>
    <property name="hibernate.connection.url">jdbc:mysql://localhost:3306/library_db</property>
    <property name="hibernate.connection.username">root</property>
    <property name="hibernate.connection.password">your_password</property>
    <property name="hibernate.dialect">org.hibernate.dialect.MySQLDialect</property>
    <property name="show_sql">true</property>
    <property name="hbm2ddl.auto">update</property>
  </session-factory>
</hibernate-configuration>
