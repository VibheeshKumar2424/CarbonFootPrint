# 🌱 Carbon Footprint Tracker

A **Spring Boot web application** that helps users track their daily **carbon footprint** based on activities like driving, electricity usage, flights, and food consumption. The application calculates CO₂ emissions, stores data securely, and presents insights with interactive charts.

---

## 🚀 Features
- 🔐 **User Authentication** – Secure login & signup with Spring Security and BCrypt password hashing  
- 📊 **Dashboard** – Displays total and activity-wise CO₂ emissions with Chart.js visualizations  
- 📝 **Activity Logging** – Add activities (car, electricity, flights, meat, etc.) with automatic emission calculation  
- 📅 **Date Tracking** – Each entry stores the date when the activity was logged  
- 👤 **Profile Page** – Shows user details and cumulative emissions  
- 🌐 **REST APIs** – Backend APIs for entries and users (future integration with mobile/React frontend)  
- 🎨 **Frontend** – Clean UI using Thymeleaf, HTML, CSS, and JavaScript  

---

## 🛠 Tech Stack
**Backend:** Spring Boot, Spring Security, Spring Data JPA  
**Frontend:** Thymeleaf, HTML, CSS, JavaScript, Chart.js  
**Database:** PostgreSQL  
**Build Tool:** Maven  
**Authentication:** BCrypt password hashing  

---

## ⚙️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/carbon-footprint-tracker.git
   cd carbon-footprint-tracker
   ```
   
Configure Database

Create a PostgreSQL database (e.g., carbonfp)

Update application.properties:

```bash
spring.datasource.url=jdbc:postgresql://localhost:5432/carbonfp
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```

Build the project

```bash
mvn clean package
```

Run the application

```bash
java -jar target/carbonfp-0.0.1-SNAPSHOT.jar
```

Access in browser

```bash
http://localhost:8080/login
```
