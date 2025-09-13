# 🎟️ Ticket System

A **Java Spring Boot application** designed for **event ticket management**.  
It demonstrates a structured Spring Boot project with clear separation of concerns, including data handling, service logic, and RESTful API endpoints.

---

## 📌 Features

- **Ticket Management**: Create, retrieve, update, and delete tickets.  
- **RESTful API**: Exposes endpoints for interacting with the ticket system.  
- **Layered Architecture**:  
  - **Ticket Class** → Represents tickets with fields like ID, event name, date, buyer name, and price.  
  - **TicketRepository** → Handles data persistence using an in-memory `Map`.  
  - **TicketService** → Business logic layer connecting the repository and controller.  
  - **TicketController** → Handles HTTP requests and maps them to service methods.  
- **Spring Boot Annotations**: Utilizes dependency injection and configuration via annotations.  

---

## 🛠️ Tech Stack

- **Java 17+**  
- **Spring Boot**  
- **Spring Web (REST API)**  
- **Maven** (build tool)  

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/Arpit-Chaurasia26/Ticket-System.git
cd Ticket-System
```

### 2️⃣ Build the Project
```bash
mvn clean install
```

### 3️⃣ Run the Application
```bash
mvn spring-boot:run
```

The application will start at:  
👉 `http://localhost:8080`

---

## 📡 API Endpoints

| HTTP Method | Endpoint               | Description                     |
|-------------|-------------------------|---------------------------------|
| **GET**     | `/tickets`             | Retrieve all tickets            |
| **GET**     | `/tickets/{id}`        | Retrieve ticket by ID           |
| **POST**    | `/tickets`             | Add a new ticket                |
| **PUT**     | `/tickets/{id}`        | Update an existing ticket       |
| **DELETE**  | `/tickets/{id}`        | Delete a ticket by ID           |

---

## 📖 Example Ticket JSON

```json
{
  "id": 1,
  "eventName": "Spring Boot Workshop",
  "date": "2025-09-15",
  "buyerName": "John Doe",
  "price": 500
}
```

---

## 🎯 Learning Outcomes

This project demonstrates:
- Organizing a Spring Boot application into **Controller, Service, Repository, and Model layers**.
- Building a **RESTful API** with CRUD operations.
- Using **Spring dependency injection** and annotations for clean and maintainable code.

---

## 🤝 Contributing

Contributions are welcome!  
If you’d like to improve this project, feel free to fork it and create a pull request.

---

## 📜 License

This project is licensed under the **MIT License**.  
You are free to use, modify, and distribute it.

---
