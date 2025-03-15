# EV-Scooter-Data-Management-System
 ## Technologies : Android Development, SpringBoot, PostgresSQL, Figma(UI/UX)

## High Level Architecture
![asdfghjh_page-0001 (2) (1)](https://github.com/user-attachments/assets/4a37751e-76dc-40a5-b9fd-b39c37b8ad0d)

## 📌 Project Overview  
This project consists of an **EV Dashboard Android app** that continuously **sends real-time vehicle data** to a **Spring Boot backend** using **Retrofit**. The backend processes and **stores the data in a PostgreSQL database**, dynamically creating tables for each vehicle based on its **VIN number**.  

Simultaneously, a **Companion Mobile App** connects to the server, requests **real-time data**, and displays it to the user, ensuring seamless monitoring and control.  

## 🛠️ Technologies Used  
- **Android (Dashboard & Companion App)** – Retrofit for API communication  
- **Spring Boot** – RESTful API backend  
- **PostgreSQL** – Database storage with dynamic VIN-based tables  
- **Cloud Deployment** – For scalable real-time data processing  
- **WebSockets/HTTP** – For real-time data transmission  

## 🔗 System Architecture  
1. **EV Dashboard App:**  
   - Continuously collects and sends **SoC, Location, Temperature, TirePressure and other telemetry data** to the backend.  
   - Uses **Retrofit** for secure and efficient data transmission.  

2. **Spring Boot Backend:**  
   - Recognizes the **phone number** linked to a vehicle via its **VIN number**.  
   - Dynamically creates a **dedicated table** for each vehicle in **PostgreSQL**.  
   - Stores incoming telemetry data in real time.  

3. **Companion Mobile App:**  
   - Authenticates the user and fetches **only the assigned vehicle’s data**.  
   - Requests real-time telemetry updates from the server.  
   - Displays key vehicle parameters such as **battery status, speed, and diagnostics**.  

## EV Dashboard ( Android App On Custom OS )
![GIFMaker_me](https://github.com/user-attachments/assets/f6cd2b6c-81e8-4b3d-9734-c5fdb5c8060c)

## Companion Mobile App (For EV Owner)

![esfrgdhj_page-0001 (1)](https://github.com/user-attachments/assets/6b053bc0-f98a-4ebe-8319-a74c0e76e18e)





