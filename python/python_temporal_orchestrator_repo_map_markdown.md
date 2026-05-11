# Python + Temporal Orchestrator Service - Repo Map

# Core Conclusion

There is no single perfect repository for enterprise orchestrator platforms.

Production-grade systems are usually built by combining:
- architecture repo
- orchestration repo
- workflow repo
- event-driven repo
- infrastructure repo

---

# Recommended Production Repo Combination

```text
ivan-borovets/fastapi-clean-example
        +
temporalio/samples-python
        +
langchain-ai/langgraph
```

This combination is strong for:
- AI orchestration
- workflow engine
- multi-agent platform
- enterprise backend
- event-driven architecture

---

# 1. Clean Architecture Foundation

## ivan-borovets/fastapi-clean-example
- Repo:
  https://github.com/ivan-borovets/fastapi-clean-example

### Purpose
- Clean Architecture
- DDD-lite
- CQRS
- Repository Pattern
- Unit Of Work
- Dependency Injection

### Use For
- enterprise service structure
- maintainable backend
- orchestration service foundation

---

# 2. Workflow Engine + Temporal Mindset

## temporalio/samples-python
- Repo:
  https://github.com/temporalio/samples-python

### Purpose
- workflow orchestration
- activity patterns
- retry patterns
- child workflows
- signals & queries
- worker scaling
- saga patterns

### Use For
- durable workflows
- orchestration engine
- long-running business process

### Important
Temporal workflows must be deterministic.
Do NOT:
- call APIs directly inside workflows
- call DB directly inside workflows
- use random or datetime.now()

All IO should be executed in activities.

---

# 3. AI Workflow + Graph Orchestration

## langchain-ai/langgraph
- Repo:
  https://github.com/langchain-ai/langgraph

### Purpose
- stateful graph execution
- checkpointing
- resumable workflows
- agent coordination
- human-in-the-loop

### Use For
- AI orchestration
- multi-agent systems
- graph-based workflow execution

---

# 4. Recommended Supporting Repositories

## FastAPI Coding Standards
### zhanymkanov/fastapi-best-practices
https://github.com/zhanymkanov/fastapi-best-practices

Use For:
- async best practices
- API conventions
- dependency management
- project organization

---

## Enterprise Infrastructure
### fastapi-practices/fastapi_best_architecture
https://github.com/fastapi-practices/fastapi_best_architecture

Use For:
- Redis
- SQLAlchemy
- Docker
- JWT/Auth
- logging
- middleware

---

## DDD + Event-Driven Mindset
### cosmicpython/code
https://github.com/cosmicpython/code

Use For:
- Repository Pattern
- Unit Of Work
- Domain Events
- Message Bus
- event-driven architecture

---

# Recommended Enterprise Stack

| Layer | Technology |
|---|---|
| API | FastAPI |
| Workflow Engine | Temporal |
| AI Orchestration | LangGraph |
| Messaging | Kafka |
| Cache | Redis |
| Database | PostgreSQL |
| ORM | SQLAlchemy 2.0 |
| Validation | Pydantic |
| Observability | OpenTelemetry |
| Deployment | Kubernetes |

---

# Recommended Folder Structure

```text
src/
 ├── workflows/
 ├── activities/
 ├── workers/
 ├── application/
 ├── domain/
 ├── infrastructure/
 ├── interfaces/
 ├── bootstrap/
 └── tests/
```

---

# Recommended Architecture Flow

```text
API Layer
    ↓
Application Layer
    ↓
Temporal Workflow
    ↓
Activities
    ↓
Infrastructure Adapters
```

---

# Important Best Practices

## DO
- keep workflows deterministic
- move all IO into activities
- separate orchestration from business logic
- use bounded contexts
- use event-driven communication
- add observability early

## DON'T
- place orchestration logic inside controllers
- build giant shared utility modules
- share mutable state across workflows
- make workflows generic for everything
- call external APIs directly inside workflows

---

# Suggested Learning Order

1. fastapi-best-practices
2. fastapi-clean-example
3. temporalio/samples-python
4. langgraph
5. cosmicpython/code
6. Kafka event-driven architecture
7. Kubernetes deployment

