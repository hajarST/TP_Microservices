Spring Cloud Microservices Project:

This GitHub repository contains a microservices project built using the Spring Cloud framework. The project consists of two microservices, service-client and service-voiture, which communicate with each other and are registered with the Eureka discovery service.

Introduction:

This project demonstrates the implementation of microservices architecture using Spring Cloud. The two microservices, service-client and service-voiture, interact with each other to maintain data consistency. The Eureka discovery service is used for service registration and discovery.


Demonstration:

![1EUREKA](https://github.com/hajarST/TP_Microservices/assets/119755584/bb40b332-fa57-4d07-857e-324bea647804)

![2Client](https://github.com/hajarST/TP_Microservices/assets/119755584/bce37b2b-4b91-4b13-98e6-294b53162ae4)

![3Voiture](https://github.com/hajarST/TP_Microservices/assets/119755584/0fabe9ab-9693-4916-a028-ad04a5523d36)

*************************************Setup:

To run the project locally, follow these steps:

Clone the repository:

Open each microservice project (service-client and service-voiture) in your preferred IDE.

Build and run each microservice.

Access the Eureka dashboard to verify that both microservices are registered:

http://localhost:8761/

**********************************Microservices Overview:
Service Client (service-client)
The service-client microservice provides CRUD operations for managing clients. It is registered with Eureka and can be accessed through the Gateway.

Service Voiture (service-voiture)
The service-voiture microservice handles operations related to cars. It communicates with the service-client to maintain client information associated with each car.

Gateway
The Gateway microservice (Gateway) serves as an entry point for accessing other microservices. It uses Spring Cloud Gateway for routing requests to the appropriate microservice.

*************************************************Usage:

Ensure that all microservices are running.

Access the Gateway service:

http://localhost:8888/

Use the provided endpoints to interact with the microservices.

********************************************Dependencies:

Spring Boot

Spring Cloud

Eureka Discovery Service

Feign for Microservice Communication
