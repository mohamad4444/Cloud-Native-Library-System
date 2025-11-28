# Cloud-Native Library Management System

This project is a lightweight library management system designed with a cloud-native architecture. It employs cutting-edge tools for orchestration, infrastructure management, service mesh, messaging, and observability.

## Overview of Technologies

### Backend Technologies

- **Java (Spring Boot)**
- **RabbitMQ**
- **Swagger** (API documentation)
- **PostgreSQL** (relational database)
### Frontend Technologies

- **HTML, CSS, TypeScript**
- **Nginx** (web server)
### Cloud & Orchestration Tools

- **Kubernetes** (orchestration)
- **Terraform** (infrastructure as code)
- **Helm** (package management)
- **Docker** (containerization)
- **Google Cloud Platform (GCP)**
### Service Mesh and Observability
- **Istio** (service mesh)
- **Jaeger** (tracing)
- **OpenTelemetry** (observability)
### Monitoring and Logging Solutions

- **Prometheus & Grafana** (monitoring and visualization)
- **SonarQube** (code quality)
- **ELK Stack** (logging: Elasticsearch, Logstash, Kibana)
### CI/CD and Automation
- **GitHub Actions** (CI/CD pipelines)
### Testing
- **JUnit** and **Mockito** (unit testing)
## Key Features
## 1. **User Management Service**

- User registration and authentication.
- Profile management.
- Role-based access control.
## 2. **Book Catalog Service**
- Add, update, and delete book entries.
- Search and filter books.
- Categorize books by genre, author, etc.
## 3. **Borrowing and Lending Service**
- Manage book checkouts and returns.
- Track due dates.
- Calculate and apply late fees.

---

# The project follows 12 Factor Methology
https://12factor.net/ <br/>
https://www.baeldung.com/spring-boot-12-factor <br/>
https://medium.com/@tech_18484/introduction-701b7a8f4730 <br/>

# Mail Service choice
dedicated mail service to generate random emails for testing and development.

Choice between:
- Mailu
  API Token : "1SS7E7LGQDIEGI2R3Y2MJ5VK2KRNCR0Z"
- Docker-Mailserver
- Modoboa
- Poste.io
- MailHog

# Mailu
https://setup.mailu.io/2024.06/

docker compose -p mailu up -d
docker compose -p mailu exec admin flask mailu admin admin mailu.io admin


# Intended Folder Structure
```
project-root/
	usermanagementService/
		backend/
			src/
			Dockerfile
			pom.xml (or build.gradle)
			application.properties
		frontend/
			public/
			src/
			package.json
			Dockerfile
	BookCatalogService/
		backend/
		frontend/
	BorrowingService/
		backend/
		frontend/
	istio/
	    gateway.yaml
	    virtualservice.yaml
	    destinationrule.yaml
```

