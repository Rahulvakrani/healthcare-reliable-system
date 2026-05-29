# Healthcare Reliable System

A comprehensive Spring Boot + Thymeleaf web application designed to solve late response and network issues in healthcare systems.

## 🎯 Features

- ✅ Patient Management
- ✅ Doctor Management  
- ✅ Medical Alerts System with retry mechanism
- ✅ Prescription Management with delivery tracking
- ✅ Automatic retry (up to 3 attempts every 30 seconds)
- ✅ Network resilience features
- ✅ Real-time Dashboard
- ✅ Responsive UI with Thymeleaf

## 🛠️ Tech Stack

- **Backend**: Spring Boot 3.1.5
- **Frontend**: Thymeleaf, HTML5, CSS3
- **Database**: MySQL
- **ORM**: Hibernate/JPA
- **Build Tool**: Maven
- **Java Version**: 17

## 📋 Prerequisites

- Java 17+
- Maven 3.6+
- MySQL 8.0+

## 🚀 Quick Start

### 1. Clone Repository
```bash
git clone https://github.com/Rahulvakrani/healthcare-reliable-system.git
cd healthcare-reliable-system
```

### 2. Setup Database
```sql
CREATE DATABASE healthcare_db;
```

### 3. Configure Database
Edit `src/main/resources/application.properties`:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/healthcare_db
spring.datasource.username=root
spring.datasource.password=your_password
```

### 4. Build & Run
```bash
mvn clean install
mvn spring-boot:run
```

Access at `http://localhost:8080/`

## 📁 Project Structure

```
healthcare-reliable-system/
├── entity/              # JPA Entities
├── repository/          # Data Access Layer
├── service/             # Business Logic
├── controller/          # Web Controllers
└── resources/           # Templates & Configs
```

## 🔄 Key Features Explained

### Network Resilience
- Automatic retry mechanism for failed deliveries
- Max 3 attempts with 30-second intervals
- Tracks delivery attempts and timestamps

### Medical Alerts
- Create and send alerts to patients
- Track delivery status
- Acknowledge alerts
- Auto-retry on network failures

### Prescription Management
- Create prescriptions for patients
- Monitor delivery status
- Track prescription lifecycle
- Auto-retry mechanism for failed deliveries

## 📊 Database Schema

- **Patients**: Patient information and medical history
- **Doctors**: Doctor profiles and specializations
- **Medical Alerts**: Alerts with delivery tracking
- **Prescriptions**: Prescriptions with delivery status

## 🤝 Contributing

Pull requests welcome! 

## 📄 License

MIT License

## 👨‍💻 Author

**Rahul Vakrani** - [@Rahulvakrani](https://github.com/Rahulvakrani)

---

**Built with ❤️ for healthcare system reliability**
