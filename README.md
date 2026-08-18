# 🏥 MediCare HealthSync — Services Parent Repository

Parent super-repository for **MediCare HealthSync Core Business Microservices**. This repository links independent business domain microservices using **Git Submodules** in a clean **Polyrepo Architecture**.

---

## 🏛️ Business Microservices Overview

```
MediCare HealthSync Business Microservices Layer
├── 👤 healthsync-patient-service      (Port 8000 - MySQL Relational Persistence & Profile Photos)
├── 👨‍⚕️ healthsync-doctor-service       (Port 8001 - MongoDB Document Directory)
└── 📋 healthsync-appointment-service  (Port 8002 - MySQL Transactional & RestClient Inter-Service Lookup)
```

---

## 🔗 Git Submodules in this Repository

| Microservice | Submodule Repository Link | Tech Stack | Storage / Inter-Service |
| :--- | :--- | :--- | :--- |
| **Patient Service** | [healthsync-patient-service](https://github.com/Matheesha-Abiman/healthsync-patient-service) | Spring Boot 3, JPA, AOP | MySQL Database + Local File Storage |
| **Doctor Service** | [healthsync-doctor-service](https://github.com/Matheesha-Abiman/healthsync-doctor-service) | Spring Boot 3, MongoDB | MongoDB Document Store |
| **Appointment Service** | [healthsync-appointment-service](https://github.com/Matheesha-Abiman/healthsync-appointment-service) | Spring Boot 3, RestClient | MySQL Database + Inter-Service Lookups |

---

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

---

## 🚀 Cloning & Local Setup

Clone this parent repository along with all its initialized microservice submodules:

```bash
git clone --recurse-submodules https://github.com/Matheesha-Abiman/medicare-healthsync-services.git
cd medicare-healthsync-services
```
