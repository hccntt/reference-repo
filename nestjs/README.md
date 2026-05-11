# NestJS Enterprise Platform - Repo Map

## 1. Core Architecture

### Domain-Driven Hexagon

* Repo: [https://github.com/Sairyss/domain-driven-hexagon](https://github.com/Sairyss/domain-driven-hexagon)
* Purpose:

  * DDD
  * Hexagonal Architecture
  * CQRS
  * Event-Driven Design
  * Enterprise Modularization
* Use For:

  * Service architecture standard
  * Domain boundary design
  * Enterprise backend foundation

---

## 2. Monorepo Management

### Nx Monorepo

* Repo: [https://github.com/nrwl/nx](https://github.com/nrwl/nx)
* Purpose:

  * Monorepo management
  * Dependency graph
  * Shared libraries
  * Incremental build
  * CI/CD optimization
* Use For:

  * Multi-service platform
  * Shared SDK/contracts
  * Enterprise scaling

---

## 3. NestJS Enterprise Boilerplate

### NestJS DDD DevOps

* Repo: [https://github.com/andrea-acampora/nestjs-ddd-devops](https://github.com/andrea-acampora/nestjs-ddd-devops)
* Purpose:

  * DDD
  * Clean Architecture
  * Kafka
  * OpenTelemetry
  * Docker
  * CI/CD
  * Observability
* Use For:

  * Production-ready backend
  * Enterprise service template
  * API Gateway architecture

---

## 4. Feature Reference Boilerplate

### Brocoders NestJS Boilerplate

* Repo: [https://github.com/brocoders/nestjs-boilerplate](https://github.com/brocoders/nestjs-boilerplate)
* Purpose:

  * Auth
  * RBAC
  * Swagger
  * Docker
  * PostgreSQL
  * Mail
  * Upload
  * Seed data
* Use For:

  * Feature reference
  * Enterprise modules
  * SaaS backend features

---

# Recommended Enterprise Stack

| Layer            | Technology    |
| ---------------- | ------------- |
| API Gateway      | NestJS        |
| Monorepo         | Nx            |
| ORM              | Prisma        |
| Messaging        | Kafka         |
| Cache            | Redis         |
| Workflow         | Temporal      |
| AI Orchestration | Python        |
| Observability    | OpenTelemetry |
| Deployment       | Kubernetes    |

---

# Recommended Folder Structure

```text
apps/
 ├── gateway
 ├── auth-service
 ├── user-service
 ├── billing-service
 ├── orchestrator-service
 └── agent-worker

libs/
 ├── shared-kernel
 ├── contracts
 ├── observability
 ├── event-bus
 ├── iam
 └── sdk
```

---

# Suggested Build Strategy

## DO:

* Use Nx for monorepo
* Use DDD + Hexagonal Architecture
* Separate bounded contexts early
* Build reusable shared libraries
* Use event-driven communication
* Add observability from the beginning

## DON'T:

* Put all business logic into gateway
* Share database across all services
* Create giant utility modules
* Mix AI orchestration into API layer
* Clone boilerplates without redesigning architecture

---

# Suggested Learning Order

1. domain-driven-hexagon
2. nx
3. nestjs-ddd-devops
4. brocoders/nestjs-boilerplate
5. Temporal + Python orchestration
6. Kafka event-driven architecture
7. Kubernetes deploy
