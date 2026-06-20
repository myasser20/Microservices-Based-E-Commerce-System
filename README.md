# E-Commerce Microservices Platform

## Overview

This project is a scalable e-commerce backend system developed using Spring Boot and Spring Cloud following a microservices architecture. The application simulates a real-world online shopping platform where users can browse products, place orders, and manage inventory through independently deployed services.

The system is designed to demonstrate modern backend development practices such as service discovery, API gateway routing, authentication and authorization, containerization, and distributed system communication.

---

## Project Goals

* Build a scalable and maintainable backend system.
* Apply microservices architecture principles.
* Implement secure authentication and authorization.
* Enable independent deployment of services.
* Demonstrate cloud-native development practices.

---

## Features

### User Authentication and Authorization

* Secure login and authentication using Keycloak.
* Role-based access control.
* Protected APIs using Spring Security.
* Token-based authentication using OAuth2 and JWT.

### API Gateway

* Single entry point for all client requests.
* Request routing to appropriate services.
* Security filtering and centralized access control.
* Simplified communication between clients and services.

### Service Discovery

* Automatic registration of services using Eureka Server.
* Dynamic discovery of service instances.
* Reduced dependency on hardcoded service URLs.

### Product Management

* Create, update, delete, and retrieve products.
* Store product details and information.
* Product search and listing capabilities.

### Order Management

* Place customer orders.
* Validate product availability.
* Process order information.
* Maintain order history.

### Inventory Management

* Track available product quantities.
* Update stock after order placement.
* Prevent ordering unavailable products.

### Database Integration

* Persistent data storage using MySQL.
* Data management with Spring Data JPA.
* Entity relationships and repository abstraction.

### Containerization

* Docker containers for each service.
* Consistent execution across environments.
* Simplified deployment process.

---

## System Architecture

The system consists of multiple independent services:

* API Gateway
* Eureka Discovery Server
* Product Service
* Order Service
* Inventory Service
* Keycloak Authentication Server
* MySQL Database

Each service has its own responsibility and can be developed, deployed, and scaled independently.

---

## Technologies Used

* Java
* Spring Boot
* Spring Cloud
* Spring Cloud Gateway
* Eureka Server
* Spring Security
* Keycloak
* OAuth2 & JWT
* Spring Data JPA
* MySQL
* Maven
* Docker
* Docker Compose

---

## Benefits of the Architecture

* Improved scalability.
* Better fault isolation.
* Easier maintenance.
* Independent deployment of services.
* Enhanced security.
* Production-ready architecture.

---

## Future Enhancements

* Kafka for asynchronous communication.
* Distributed tracing with Zipkin.
* Centralized logging.
* Kubernetes deployment.
* CI/CD pipeline integration.
* Payment service integration.
* Notification service.
* Monitoring with Prometheus and Grafana.

---
## Project Structure

ecommerce-microservices/

│── api-gateway/

│── discovery-server/

│── product-service/

│── order-service/

│── inventory-service/

│── docker-compose.yml

## Running the Project

Clone the repository
git clone https://github.com/your-username/ecommerce-microservices.git

# Build the services
mvn clean install

## Run with Docker
docker-compose up -d

## Service Ports
API Gateway | 8080
Eureka Server	| 8761
Product Service	| 8081
Order Service	| 8082
Inventory Service |	8083
Keycloak	| 8181


