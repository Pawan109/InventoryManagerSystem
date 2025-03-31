# Inventory Management System (Spring Boot + Kafka)  

### **Overview**  
This project has a beginner-friendly Proof of Concept (POC) for an **Inventory Management System**.

It introduces core **Spring Boot** concepts like creating RESTful APIs, integrating a relational database, building microservices, and asynchronous communication via Kafka.  

By working on this project, I understood how to structure scalable systems, implement business logic, and design better solutions before writing code.  

---

### **Features**  
- **Microservices**: Independent services for Order and Product management.  
- **RESTful APIs**: Simple and efficient communication between services.  
- **Database Integration**: Use Spring Data JPA to interact with a relational database.  
- **Kafka Messaging**: Asynchronous communication between microservices.  
- **Design-First Approach**: Building sequence diagrams to plan the system flow.  

---

### **System Workflow**  
1. **Order Placement**: Users place orders with multiple products.  
2. **Availability Check**: Each product's stock is checked with the Product Service.  
3. **Event-Driven Updates**: The system publishes events (Order Placed, Out of Stock) using Kafka.  
4. **Inventory Updates**: Product Service updates stock levels asynchronously.  
5. **Order Status Update**: Real-time updates provided to users.  

---

### **Key Components**  

#### 1. **Order Service**  
- Handles incoming order requests.  
- Adjusts orders if products are unavailable.  
- Publishes events to Kafka on successful or failed order placement.  

#### 2. **Product Service**  
- Manages inventory data and updates stock levels.  
- Listens to Kafka events to handle inventory changes.  

#### 3. **Kafka Integration**  
- Ensures reliable communication between services.  
- Enables scalability and resilience through asynchronous messaging.  

---

### **Diagrams**

![image](https://github.com/user-attachments/assets/8edbb125-aea5-45e7-b6ed-2d4feef9167b)



![image](https://github.com/user-attachments/assets/8a199895-f7cf-4435-baec-652148fbfb6d)


### **Technologies Used**  
- **Backend**: Spring Boot, Spring Data JPA, Kafka  
- **Database**: MySQL  
- **Messaging**: Apache Kafka  
- **Tools**: Postman (API testing), Docker 

---

### **Projects Goals**  
- **Understand Microservices**: Learning how to create and run independent services.  
- **Explore Kafka**: Dive into event-driven architecture.  
- **Learn Design Skills**: Create sequence diagrams to visualize system flows.  
- **Develop Real-World Systems**: Gaining hands-on experience in building scalable and robust systems.  


