# OptiCuter Solution

OptiCuter is a microservices-based solution built using Go (Golang) and deployed on Google Cloud Platform (GCP) using Docker containers and Kubernetes (K8s). The project integrates several services, including user management, material management, real-time chat, video calls, notifications, and more. It utilizes multiple databases and real-time technologies such as WebSockets for chat and Jitsi for video calls.

## Project Overview

The OptiCuter solution consists of the following services:

- **User Service**: Manages user information, authentication, and profiles.
- **Material Service**: Handles operations related to materials, including storage, retrieval, cutting results, and payments.
- **Admin Service**: Provides administrative functionalities, such as user management and data oversight.
- **Chat Service**: Enables real-time messaging and communication through WebSockets and integrates Jitsi for video calls.
- **Notification Service**: Sends notifications via email (SMTP) and uses Kafka for event-driven notifications across services.
- **API Gateway Service**: Acts as the entry point for the entire system, routing requests to the appropriate microservices.

## Technologies Used

- **Go (Golang)**: Backend language for building the microservices.
- **PostgreSQL**: Used for storing structured relational data.
- **MongoDB**: Used for chat message storage and other unstructured data.
- **Redis**: Utilized for OTP and order ID storage.
- **SMTP**: Email notifications for alerts and communication.
- **Kafka**: Event streaming to facilitate asynchronous communication between services.
- **WebSocket**: Real-time communication for the chat service.
- **Jitsi**: Integrated for video call services.
- **Docker**: Containers for service isolation and deployment.
- **Kubernetes (K8s)**: Orchestration platform for service deployment and scaling.
- **GCP (Google Cloud Platform)**: Cloud environment for scalable deployment and management.

## Features

- **Microservices Architecture**: Services are decoupled, allowing independent scaling and maintenance.
- **Real-Time Communication**: Chat functionality powered by WebSockets and video calls via Jitsi.
- **Event-Driven Communication**: Kafka enables loose coupling and event streaming across services.
- **Scalability & High Availability**: Kubernetes ensures that services are scalable and resilient, while Docker containers simplify deployment and management.

## Getting Started

### Prerequisites

Before setting up the project, make sure you have the following tools installed on your local machine:

- **Go 1.23.1** or higher (matching the version used in the project).
- **Docker**: For containerizing the services.
- **Kubernetes (kubectl)**: To manage and deploy services on Kubernetes clusters.
- **GCP CLI**: For managing resources and deploying the project to GCP.

### Setup and Deployment

1. **Clone the repository**:
   First, clone the repository to your local machine:
   ```bash
   git clone https://github.com/ratheeshkumar25/opti_cutter_final.git
   cd opti_cuter-chat
