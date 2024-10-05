# Automatic Attendance System using Face Recognition

## Overview
This project is a cross-platform mobile application that automates the attendance process using facial recognition technology. Users can register themselves, and the system will log their attendance using their face as identification. It is built using **React Native** for the frontend, **Spring Boot** for the backend, and **MongoDB** for data storage. The project ensures secure authentication, efficient data management, and accurate real-time face recognition using **OpenCV**.

## Features
- **User Registration & Login**: Users can securely register and log in to the app using a JWT-based authentication system.
- **Face Recognition**: Integrated facial recognition using OpenCV for accurate user identification and attendance logging.
- **Attendance Logging**: Automates attendance logging and stores detailed records of attendance.
- **Role-based Access Control**: Different levels of access for admins and users (professors, students).
- **Scalable and Efficient**: Built with a modular architecture for scalability and optimized for efficient database interactions.

## Technologies
- **Frontend**: React Native
- **Backend**: Spring Boot
- **Database**: MongoDB
- **Facial Recognition**: OpenCV
- **Authentication**: JWT (JSON Web Token)
- **APIs**: RESTful API services

## Requirements
### Backend:
- Java 11+
- Spring Boot
- MongoDB
- Maven

### Frontend:
- React Native CLI
- Node.js (v14+)
- OpenCV (for facial recognition integration)
- Android Studio or Xcode for emulation

### Database:
- MongoDB Community Server

## Installation

### Backend Setup (Spring Boot)
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/attendance-system-backend.git

2. Clone the repository:
   ```bash
   cd attendance-system-backend
3. Build the project using Maven:
   ```bash
   mvn clean install
4. Build the project using Maven:
   ```bash
   mvn spring-boot:run

### Frontend Setup (React Native)
1. Clone the frontend repository:
   ```bash
   git clone https://github.com/your-username/attendance-system-frontend.git
   
2. Navigate to the project directory:
   ```bash
   cd attendance-system-frontend
   
3. Install dependencies:
   ```bash
   mvn clean install

4. Start the React Native app
   ```bash
   npx react-native run-android  # for Android
   npx react-native run-ios      # for iOS

   
   
