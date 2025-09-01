# 🚌 Bus Tracking System

## 🚀 Overview
The **Bus Tracking System** is a full-stack application that allows passengers, drivers, and administrators to manage and track buses in real-time.  
- **Passengers** can view routes, track live bus locations, and get estimated arrival times.  
- **Drivers** can update their location as they move.  
- **Admins** can manage buses, routes, and drivers.  

This project demonstrates **end-to-end development** using Java (Spring Boot) for the backend, React for the frontend, MySQL for data storage, and WebSockets for real-time tracking.

---

## ⚙️ Tech Stack
### Frontend
- React  
- React Router  
- Axios  
- Google Maps API / Leaflet.js  
- Material UI / Bootstrap  

### Backend
- Java 17+  
- Spring Boot (REST APIs)  
- Spring Security + JWT (Authentication & Authorization)  
- Spring Data JPA (Database Access)  
- WebSocket (Real-time location updates)  

### Database
- MySQL (or PostgreSQL)  

### Deployment
- Backend → AWS Elastic Beanstalk / Render  
- Frontend → Vercel / Netlify  
- Database → AWS RDS / ElephantSQL


## 📂 Project Structure
---

bus-tracking-system/
├── backend/ # Spring Boot APIs
├── frontend/ # React UI
└── docs/ # Diagrams & documentation



---

## ✨ Features
### 👩‍💻 Passenger
- User registration & login  
- View available buses & routes  
- Track bus live location on map  
- Get estimated arrival time  

### 👨‍✈️ Driver
- Login & location updates (via GPS/mobile)  

### 🛠️ Admin
- Manage buses, routes, and drivers  
- View reports (usage, trips, delays)  

---

## 🏗️ System Architecture
**High-Level Flow:**  
1. Passenger/Driver/Admin logs in.  
2. React frontend interacts with Spring Boot backend via REST APIs.  
3. Backend stores data in MySQL & manages authentication with JWT.  
4. Driver location updates are sent to backend → broadcasted via WebSocket → passengers see real-time bus position on map.  

---

## 📊 Database Design (Initial)
- **Users**: id, name, email, password, role  
- **Buses**: id, bus_number, route_id, driver_id  
- **Drivers**: id, name, phone, bus_id  
- **Routes**: id, start_point, end_point, stops[]  
- **Locations**: bus_id, latitude, longitude, timestamp  

---

## 🚀 Setup Instructions
### Backend
1. Clone repo & navigate to `/backend`  
2. Update `application.properties` with DB credentials  
3. Run Spring Boot app → `mvn spring-boot:run`  

### Frontend
1. Navigate to `/frontend`  
2. Install dependencies → `npm install`  
3. Start app → `npm start`  

---

## 📸 Demo (To Be Added)
- Screenshots of UI  
- Short video demo  

---

## 📌 Future Enhancements
- Push notifications for bus arrival alerts  
- QR code check-in for passengers  
- AI-based ETA predictions using traffic history  

---

## 👨‍💻 Author
CHINNASAMY R
📧 chinnasamyramesh8524@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/chinnasamyramesh8524/) | [GitHub](https://github.com/chinnasamyramesh8524)
