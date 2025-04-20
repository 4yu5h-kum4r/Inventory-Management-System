# Inventory-Management-System
An Inventory Management System built with React and Springboot along with ElectronJS to run as desktop application. It is used to manage inventory of a shop. It is  just a smaller ERP tool.


A desktop-based inventory management system built using:

- **Spring Boot** (Java) for the backend
- **ReactJS** (with Electron) for the frontend
- **H2 database** (embedded, file-based, no internet required)

This application is designed to run locally at a single shop without requiring an internet connection.

---

## Features

- Desktop GUI using Electron
- Offline support with embedded H2 database
- Product entry via UI or Excel upload
- CRUD operations for inventory items
- Basic authentication (optional, configurable)
- Easy packaging into a single `.exe` for Windows

---

## Project Structure

```
Inventory-Management-System
├── backend/ # Spring Boot backend 
├── frontend/ # React + Electron frontend
├── data/ # H2 DB files (generated at runtime)
├── .gitignore
└── README.md
```
---

## Prerequisites

- **Java 17+**
- **Node.js 16+**
- **Maven** (for building backend)
- **Yarn** or **npm** (for frontend)
- **Electron Packager** (for packaging app)

---

## Run Instructions

### 1. Backend (Spring Boot)

```
cd backend
mvn clean package
java -jar target/inventory-0.0.1-SNAPSHOT.jar
```

### 2. Frontend (React + Electron)

```
cd frontend
npm install
npm start
```

This will launch the Electron desktop window pointing to ```http://localhost:8080```.

### 3. Packaging the App

```
cd frontend
npm run package
```
The ```.exe``` will be created under the ```release/``` folder.


---
## Author
Ayush Kumar
