```markdown id="rd1"
# Booking System Config Repository

This repository contains centralized configuration files for all microservices in the Booking System.

It is used by Spring Cloud Config Server to externalize and manage configurations in a distributed microservices architecture.

## 📦 Purpose

- Centralized configuration management
- Environment-independent configuration
- Dynamic configuration updates without redeployment
- Support for microservices architecture

## 🏗️ Services Covered

- api-gateway
- user-service
- booking-service
- payment-service
- notification-service

## 📂 Structure


booking-system-config-repo/
├── application.yml
├── api-gateway.yml
├── user-service.yml
├── booking-service.yml
├── payment-service.yml
├── notification-service.yml


## ⚙️ How It Works

1. Spring Cloud Config Server connects to this Git repository
2. Each microservice requests its configuration from the Config Server
3. Config Server serves the corresponding YAML file based on the service name

## 🔐 Notes

- Avoid storing sensitive data directly in this repository
- Use environment variables or secret management tools in production
- This repository should be version-controlled like source code

## 🚀 Technologies

- Spring Cloud Config
- Git-based configuration
- YAML configuration format

---

Maintained as part of the Booking System microservices architecture.
```
