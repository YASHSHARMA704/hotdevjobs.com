# HotDevJobs.com

**HotDevJobs.com** is a modern job listing platform tailored for developers. It allows job seekers to find high-quality developer jobs and provides a space for employers to post opportunities and attract top engineering talent.

## 🚀 Features

- 🔍 Curated developer job listings
- 🔎 Search and filter by keywords and location
- 📱 Fully responsive design
- 🔐 Secure user authentication (login & registration)
- 📝 Job posting interface for employers
- 📂 Application tracking for job seekers

## 🛠️ Tech Stack

### Frontend
- HTML5, CSS3, JavaScript
- Thymeleaf (Server-side templating)

### Backend
- Java 17
- Spring Boot 3
- Spring MVC
- Spring Security
- Spring Data JPA

### Database
- MySQL

### Build Tool
- Maven

## ⚙️ Installation

### Prerequisites

- Java 17+
- Maven 3+
- MySQL Server
- IDE (IntelliJ IDEA, Eclipse, etc.)

### Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/YASHSHARMA704/hotdevjobs.com.git
   cd hotdevjobs.com
2. **Create MySQL Database**
    Open your MySQL client (e.g., MySQL CLI, MySQL Workbench) and execute the following commands to set up the database and user:
   ```bash
    CREATE DATABASE hotdevjobs;
    CREATE USER 'hotdevuser'@'localhost' IDENTIFIED BY 'yourpassword';
    GRANT ALL PRIVILEGES ON hotdevjobs.* TO 'hotdevuser'@'localhost';
    FLUSH PRIVILEGES;
   ```
3. **Configure Application Properties**

    Locate the application.properties file at:
   ```bash
   src/main/resources/application.properties
   ```
   Replace the default values with your actual MySQL credentials:
   ```bash
    spring.datasource.url=jdbc:mysql://localhost:3306/hotdevjobs
    spring.datasource.username=hotdevuser
    spring.datasource.password=yourpassword
    spring.jpa.hibernate.ddl-auto=update
   ```
4. **Build and Run the Application**
    Run the following Maven commands in your terminal to build and launch the Spring Boot application:
   ```bash
    mvn clean install
    mvn spring-boot:run
   ```
