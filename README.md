# ConnectSphere – Microservices Based Professional Networking Platform

ConnectSphere is a microservices-based backend platform designed to simulate a professional networking system similar to modern social platforms.
The system is built using **Java 21, Spring Boot, and Spring Cloud** and follows a scalable microservices architecture.

It allows users to create profiles, publish posts, connect with other professionals, and receive notifications through independent services communicating via service discovery and API gateway.

---

## Tech Stack

* Java 21
* Spring Boot
* Spring Cloud
* Spring Security
* Spring Data JPA
* REST APIs
* Docker (for containerization)
* Kubernetes (deployment configs)

---

## Microservices Architecture

The platform follows a distributed microservices architecture.

API Gateway
↓
Service Discovery (Eureka Server)
↓
User Service
Post Service
Connection Service
Notification Service

Each service is independently deployable and communicates through REST APIs

---
Services Overview
API Gateway

Acts as a single entry point for all client requests and routes them to the appropriate microservices.

Discovery Server

Service registry using Spring Cloud Eureka that allows services to register and discover each other dynamically.

User Service

Handles user profiles, registration, and profile management.

Posts Service

Manages user posts and feed-related functionality.

Connections Service

Handles connection requests and networking between users.

Notification Service

Responsible for sending notifications when users receive connection requests, likes, or other updates.

---
Project Structure

connectsphere-microservices

api-gateway
connections-service
discovery-server
notification-service
posts-service
user-service

---
Key Features

Microservices architecture

Service discovery with Eureka

API Gateway for routing

Scalable backend design

Independent service deployment

Professional networking workflow

---
How to Run

Clone the repository

git clone https://github.com/Zeeshan9980/connectsphere-microservices.git

Navigate to the project

cd connectsphere-microservices

Run services individually using your IDE or build tool.

---
Author

Zeeshan Ahmed
Java Backend Developer

LinkedIn
https://www.linkedin.com/in/zeeshan-ahmed-b9a2a222b/

---
Purpose of the Project

This project was built to demonstrate microservices architecture using Spring Boot and Spring Cloud while simulating a real-world professional networking platform.
