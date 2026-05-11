# Python Enterprise Backend - Repo Map

## 1. Clean Architecture + DDD

### ivan-borovets/fastapi-clean-example

* Repo: [https://github.com/ivan-borovets/fastapi-clean-example](https://github.com/ivan-borovets/fastapi-clean-example)
* Purpose:

  * Clean Architecture
  * DDD-lite
  * CQRS
  * Dependency Injection
  * Unit Of Work
  * Repository Pattern
* Use For:

  * Enterprise backend
  * AI platform services
  * Long-term maintainability

---

## 2. Enterprise FastAPI Architecture

### fastapi-practices/fastapi_best_architecture

* Repo: [https://github.com/fastapi-practices/fastapi_best_architecture](https://github.com/fastapi-practices/fastapi_best_architecture)
* Purpose:

  * Async architecture
  * Redis
  * JWT/Auth
  * SQLAlchemy
  * Docker
  * Middleware
  * Logging
* Use For:

  * Production API
  * Enterprise backend
  * Internal services

---

## 3. FastAPI Coding Standards

### zhanymkanov/fastapi-best-practices

* Repo: [https://github.com/zhanymkanov/fastapi-best-practices](https://github.com/zhanymkanov/fastapi-best-practices)
* Purpose:

  * Async best practices
  * API layering
  * Validation
  * Dependency Injection
  * Project organization
* Use For:

  * Coding conventions
  * Team standards
  * Async service development

---

## 4. Hexagonal Architecture Python

### szymon6927/hexagonal-architecture-python

* Repo: [https://github.com/szymon6927/hexagonal-architecture-python](https://github.com/szymon6927/hexagonal-architecture-python)
* Purpose:

  * Ports/Adapters
  * CQRS
  * Event-driven architecture
  * Domain isolation
* Use For:

  * Enterprise microservices
  * Bounded contexts
  * Event-driven systems

---

## 5. Production Reference API

### nsidnev/fastapi-realworld-example-app

* Repo: [https://github.com/nsidnev/fastapi-realworld-example-app](https://github.com/nsidnev/fastapi-realworld-example-app)
* Purpose:

  * Production API implementation
  * JWT/Auth
  * SQLAlchemy async
  * CRUD patterns
* Use For:

  * Production coding style
  * API implementation reference

---

## 6. Dependency Injection

### ets-labs/python-dependency-injector

* Repo: [https://github.com/ets-labs/python-dependency-injector](https://github.com/ets-labs/python-dependency-injector)
* Purpose:

  * Dependency Injection
  * Container management
  * Modular architecture
* Use For:

  * Large systems
  * Multi-service architecture
  * Testable enterprise code

---

## 7. Async SQLAlchemy Best Practices

### rhoboro/async-fastapi-sqlalchemy

* Repo: [https://github.com/rhoboro/async-fastapi-sqlalchemy](https://github.com/rhoboro/async-fastapi-sqlalchemy)
* Purpose:

  * Async SQLAlchemy 2.0
  * Transaction management
  * Repository pattern
* Use For:

  * Async DB architecture
  * Enterprise persistence layer

---

## 8. DDD + Architecture Mindset

### cosmicpython/code

* Repo: [https://github.com/cosmicpython/code](https://github.com/cosmicpython/code)
* Purpose:

  * Repository Pattern
  * Unit Of Work
  * Domain Events
  * Message Bus
  * DDD patterns
* Use For:

  * Enterprise architecture mindset
  * Event-driven backend
  * Workflow-oriented systems

---

# Recommended Enterprise Python Stack

| Layer                | Technology          |
| -------------------- | ------------------- |
| API                  | FastAPI             |
| ORM                  | SQLAlchemy 2.0      |
| Validation           | Pydantic            |
| Migration            | Alembic             |
| Workflow             | Temporal            |
| Messaging            | Kafka               |
| Cache                | Redis               |
| Dependency Injection | dependency-injector |
| Observability        | OpenTelemetry       |
| Deployment           | Kubernetes          |

---

# Recommended Folder Structure

```text
src/
 ├── application/
 ├── domain/
 ├── infrastructure/
 ├── interfaces/
 ├── bootstrap/
 └── tests/
```

---

# Avoid This Structure

```text
routers/
services/
models/
utils/
```

Problems after scaling:

* circular imports
* god services
* hard testing
* difficult maintenance

---

# Recommended Repo Combination

| Goal                      | Repository                          |
| ------------------------- | ----------------------------------- |
| Clean Architecture        | ivan-borovets/fastapi-clean-example |
| Coding Standards          | zhanymkanov/fastapi-best-practices  |
| Enterprise Infrastructure | fastapi_best_architecture           |
| DDD Mindset               | cosmicpython                        |

---

# Suggested Learning Order

1. fastapi-best-practices
2. fastapi-clean-example
3. fastapi_best_architecture
4. cosmicpython/code
5. dependency-injector
6. Temporal + Kafka architecture
