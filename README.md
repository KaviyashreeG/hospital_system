# Hospital Management System

A comprehensive full-stack application for managing hospital operations, featuring role-based dashboards for Patients, Doctors, and Administrators.

## 🔗 Live Demo
- **Frontend**: [https://hospital-system-three-hazel.vercel.app](https://hospital-system-three-hazel.vercel.app)
- **Backend API**: [https://med-flow.onrender.com](https://med-flow.onrender.com)

## 🚀 Features

- **Role-Based Access Control**: Secure authentication and authorization using Spring Security and JWT.
  - **Admin**: Manage doctors, patients, and hospital departments.
  - **Doctor**: View assigned appointments, manage availability slots, and handle patient cases.
  - **Patient**: Register, browse departments/doctors, book appointments, and view appointment history.
- **Appointment Booking System**: Patients can view available slots and book appointments with doctors.
- **Interactive Dashboards**: Dedicated UI dashboards (Admin, Doctor, Patient) built with React.
- **RESTful API**: Robust backend API built with Spring Boot.
- **Database**: PostgreSQL integration for reliable data persistence.

## 🛠️ Tech Stack

### Backend
- **Framework**: Spring Boot 3
- **Language**: Java 17
- **Database**: PostgreSQL (Supabase)
- **Security**: Spring Security + JWT (JSON Web Tokens)
- **Data Access**: Spring Data JPA / Hibernate
- **Build Tool**: Maven
- **API Documentation**: Swagger / OpenAPI 3

### Frontend
- **Library**: React 19
- **Routing**: React Router DOM v7
- **Styling**: Vanilla CSS for flexible and custom designs
- **Testing**: React Testing Library & Jest

## ⚙️ Prerequisites

Before you begin, ensure you have the following installed on your machine:
- [Java Development Kit (JDK) 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Node.js and npm](https://nodejs.org/)
- [Maven](https://maven.apache.org/) (optional, as the project includes Maven Wrapper)
- A running instance of PostgreSQL (or use the provided Supabase configuration in `application.properties`).

## 🏃‍♂️ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/KaviyashreeG/hospital_system.git
cd hospital_system
```

### 2. Setup the Backend

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Configure your database connection in `src/main/resources/application.properties` if you wish to use a local PostgreSQL instance. Otherwise, it is pre-configured to use Supabase.
3. Build and run the Spring Boot application:
   ```bash
   # Using Maven Wrapper (Windows)
   mvnw spring-boot:run

   # Using Maven Wrapper (Mac/Linux)
   ./mvnw spring-boot:run
   ```
4. The backend API will start on `http://localhost:8080`.
5. You can view the API documentation at `http://localhost:8080/swagger-ui.html` (once running).

### 3. Setup the Frontend

1. Open a new terminal and navigate to the frontend directory:
   ```bash
   cd frontend
   ```
2. Install the dependencies:
   ```bash
   npm install
   ```
3. Start the React development server:
   ```bash
   npm start
   ```
4. The frontend application will open in your browser at `http://localhost:3000`.

## 📁 Project Structure

```
hospital_system/
├── backend/                  # Spring Boot application
│   ├── src/main/java/...     # Java source code (Controllers, Services, Entities, etc.)
│   ├── src/main/resources/   # Properties and static resources
│   └── pom.xml               # Maven dependencies
└── frontend/                 # React application
    ├── src/components/       # React components (Dashboards, Auth pages, etc.)
    ├── package.json          # Node dependencies
    └── ...
```

## 🤝 Contributing

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
