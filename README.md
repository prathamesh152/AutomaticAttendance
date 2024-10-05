Automatic Attendance System using Face Recognition
Overview
This project is a cross-platform mobile application that automates the attendance process using facial recognition technology. Users can register themselves, and the system will log their attendance using their face as identification. It is built using React Native for the frontend, Spring Boot for the backend, and MongoDB for data storage. The project ensures secure authentication, efficient data management, and accurate real-time face recognition using OpenCV.

Features
User Registration & Login: Users can securely register and log in to the app using a JWT-based authentication system.
Face Recognition: Integrated facial recognition using OpenCV for accurate user identification and attendance logging.
Attendance Logging: Automates attendance logging and stores detailed records of attendance.
Role-based Access Control: Different levels of access for admins and users (professors, students).
Scalable and Efficient: Built with a modular architecture for scalability and optimized for efficient database interactions.
Technologies
Frontend: React Native
Backend: Spring Boot
Database: MongoDB
Facial Recognition: OpenCV
Authentication: JWT (JSON Web Token)
APIs: RESTful API services
Requirements
Backend:
Java 11+
Spring Boot
MongoDB
Maven
Frontend:
React Native CLI
Node.js (v14+)
OpenCV (for facial recognition integration)
Android Studio or Xcode for emulation
Database:
MongoDB Community Server
Installation
Backend Setup (Spring Boot)
Clone the repository:
bash
Copy code
git clone https://github.com/your-username/attendance-system-backend.git
Navigate to the project directory:
bash
Copy code
cd attendance-system-backend
Build the project using Maven:
bash
Copy code
mvn clean install
Run the Spring Boot application:
bash
Copy code
mvn spring-boot:run
Ensure MongoDB is running locally or configure your MongoDB URI in the application.properties file:
properties
Copy code
spring.data.mongodb.uri=mongodb://localhost:27017/attendance
Frontend Setup (React Native)
Clone the frontend repository:
bash
Copy code
git clone https://github.com/your-username/attendance-system-frontend.git
Navigate to the project directory:
bash
Copy code
cd attendance-system-frontend
Install dependencies:
bash
Copy code
npm install
Start the React Native app:
bash
Copy code
npx react-native run-android  # for Android
npx react-native run-ios      # for iOS
Setting Up OpenCV for Facial Recognition
Install OpenCV:
For Android, configure the build.gradle file to include OpenCV.
For iOS, add OpenCV framework support.
Ensure the backend processes images for face recognition through integrated OpenCV libraries.
Test face recognition accuracy during user registration and attendance logging.
API Endpoints
User Endpoints
POST /api/register: Register a new user with name, email, and face data.
POST /api/login: User login using email and password.
Attendance Endpoints
POST /api/attendance/log: Log attendance for the user with facial recognition.
GET /api/attendance/{userId}: Retrieve attendance records for a specific user.
Authentication & Security
JWT Authentication: Used for securing API endpoints.
Role-Based Access Control: Admin, Professor, and Student roles with different levels of access.
Data Privacy: Sensitive information, including facial recognition data, is encrypted and securely stored in MongoDB.
Running Tests
Unit and integration tests can be run using:
bash
Copy code
mvn test
Frontend testing can be done using tools like Jest and React Native Testing Library.
Future Enhancements
Notifications: Add push notifications for attendance reminders.
Analytics Dashboard: For admins to monitor attendance trends.
Offline Mode: Support offline attendance logging and sync when the device is back online.
