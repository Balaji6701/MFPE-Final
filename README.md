# Collateral Loans – Risk Assessment
### MFPE

Collateral Loans - Risk Assessment is a miroservice architecture based application powered by spring boot.
The backend is fully powered by Java-Spring boot and front-end is made using Angular
## Requirements
- Spring boot 2.7.0
- Angular 12
- Docker
- PostMan desktop
- Spring tool suite

## Back-End services
- Authorization-Service
- Loan-Management-Service
- Collateral-Management-Service
- Risk-Assessment-Service

## Front-End
- Loan-Management-App

## Features
- Managing Loan Details for customers.
- Manage Collaterals associated with the Loan.
- Assess risks percentage for a particular Collateral.
- Secured by **JWT** authorization using **Spring security**.
- Microservice architecture.
- Dockerized

## Deployment steps
- Every service is commited to a **AWS Code-Commit** repository.
- Every service has its own **AWS Code-Pipe** line to enable.
- After build the services will be pushed to **AWS Elastic Container Registry** as docker images.
- After the build of every service is successfull, Run the **docker-compose.yml** file using following commands.
### Prerequisite
- Configure aws credential
- Install aws cli version 2
- Switch to folder where docker-compose.yml is present
```
docker context create ecs pod1-ecs
docker context use pod1-ecs
docker compose up
```
- This will create a **AWS CloudFormation Stack**, which will deploy all the services to the **AWS Elastic Container Services**.

