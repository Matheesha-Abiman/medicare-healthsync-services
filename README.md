# 🏥 MediCare HealthSync — Services Parent Repository

Parent repository for the MediCare HealthSync core business microservices. The repository uses a Polyrepo architecture with Git Submodules for the Patient, Doctor, and Appointment services.

## Student Information

| Field | Details |
|---|---|
| Student Name | Matheesha Abiman |
| Student Number | 241722050 |
| Slack Handle | Matheesha Abiman |
| GCP Project ID | medicare-healthsync-project |

## Project Description

This repository groups the three core business microservices of MediCare HealthSync:

- Patient Service
- Doctor Service
- Appointment Service
  

## 🏛️ Business Microservices Overview

```
MediCare HealthSync Business Microservices Layer
├── 👤 healthsync-patient-service      (Port 8000 - MySQL Relational Persistence & Profile Photos)
├── 👨‍⚕️ healthsync-doctor-service       (Port 8001 - MongoDB Document Directory)
└── 📋 healthsync-appointment-service  (Port 8002 - MySQL Transactional & RestClient Inter-Service Lookup)
```

## Architecture

```text
MediCare HealthSync
        |
        v
Services Parent Repository
        |
        +--> healthsync-patient-service
        |       Port 8000
        |       MySQL
        |
        +--> healthsync-doctor-service
        |       Port 8001
        |       MongoDB
        |
        +--> healthsync-appointment-service
                Port 8002
                MySQL
                RestClient
```

---

## 🔗 Git Submodules in this Repository

| Microservice | Submodule Repository Link | Tech Stack | Storage / Inter-Service |
| :--- | :--- | :--- | :--- |
| **Patient Service** | [healthsync-patient-service](https://github.com/Matheesha-Abiman/healthsync-patient-service) | Spring Boot 3, JPA, AOP | MySQL Database + Local File Storage |
| **Doctor Service** | [healthsync-doctor-service](https://github.com/Matheesha-Abiman/healthsync-doctor-service) | Spring Boot 3, MongoDB | MongoDB Document Store |
| **Appointment Service** | [healthsync-appointment-service](https://github.com/Matheesha-Abiman/healthsync-appointment-service) | Spring Boot 3, RestClient | MySQL Database + Inter-Service Lookups |

---


## Technology Stack

- Java
- Spring Boot 3
- Spring Cloud
- Maven
- REST APIs
- Git and GitHub
- Google Cloud Platform (GCP)

## Getting Started

### Prerequisites

- JDK 21 or 25
- Maven
- Git
- MySQL and/or MongoDB as required by the service
- Node.js and npm for the web application
- GCP access for cloud deployment

### Clone

```bash
git clone <REPOSITORY_URL>
cd <REPOSITORY_FOLDER>
```

### Clone With Submodules

```bash
git clone --recurse-submodules https://github.com/Matheesha-Abiman/medicare-healthsync-services.git
cd medicare-healthsync-services
```

If already cloned without submodules:

```bash
git submodule update --init --recursive
```

## Related Repositories

- `medicare-healthsync-platform`
- `medicare-healthsync-webapp`
- `healthsync-api-gateway`
- `healthsync-config-server`
- `healthsync-service-registry`


## 📦 Complete 9-Repository Polyrepo Blueprint

### Parent Repositories
- 🌐 [medicare-healthsync-platform](https://github.com/Matheesha-Abiman/medicare-healthsync-platform)
- 💼 [medicare-healthsync-services](https://github.com/Matheesha-Abiman/medicare-healthsync-services)

### Frontend Web Application
- 🖥️ [medicare-healthsync-webapp](https://github.com/Matheesha-Abiman/medicare-healthsync-webapp)

### Platform Submodules
- 🌉 [healthsync-api-gateway](https://github.com/Matheesha-Abiman/healthsync-api-gateway)
- ⚙️ [healthsync-config-server](https://github.com/Matheesha-Abiman/healthsync-config-server)
- 📡 [healthsync-service-registry](https://github.com/Matheesha-Abiman/healthsync-service-registry)

### Microservices Submodules
- 📋 [healthsync-appointment-service](https://github.com/Matheesha-Abiman/healthsync-appointment-service)
- 👨‍⚕️ [healthsync-doctor-service](https://github.com/Matheesha-Abiman/healthsync-doctor-service)
- 👤 [healthsync-patient-service](https://github.com/Matheesha-Abiman/healthsync-patient-service)

  ## Repository Role

This is the Backend Services Parent Repository for the MediCare HealthSync Polyrepo architecture.


Parent super-repository for **MediCare HealthSync Core Business Microservices**. This repository links independent business domain microservices using **Git Submodules** in a clean **Polyrepo Architecture**.



