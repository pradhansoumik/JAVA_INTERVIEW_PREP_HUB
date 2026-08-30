## Microservices Topics

- Monolithic vs Microservices Architecture
- Features/Characteristics of Microservices
  - Single Responsibility / focused on one business capability
  - Independently deployable services
  - Decentralized data management (Database per Service)
  - Decentralized governance (polyglot language/DB where useful)
  - Smart endpoints & dumb pipes (lightweight HTTP/messaging, not ESB)
  - Design for failure (timeouts, retries, circuit breaker, fallback)
  - Infrastructure automation (CI/CD, containers, K8s/OCP)
  - Observable (logs, metrics, traces, health)
  - Evolutionary design (Strangler, incremental split from monolith)
  - Organized around business capabilities / bounded contexts (DDD)
  - Loose coupling & high cohesion (API/events as contracts)
  - Scalability per service (scale hot services independently)
  - Team autonomy (often aligned with Conway’s Law / two-pizza teams)
- Communication between Microservices (sync/async, Gateway vs S2S)
  - Notes: `MICROSERVICE-DESIGN-PATTERNS/00-fundamentals/01-SERVICE-COMMUNICATION.md`
- Security — Authentication & Authorization (JWT, Gateway, mTLS)
  - Notes: `MICROSERVICE-DESIGN-PATTERNS/00-fundamentals/02-SECURITY-AUTHN-AUTHZ.md`
- Microservices Design Patterns
  1. Decomposition Patterns
       - Decompose by Business Capability
       - Decompose by Subdomain
       - **Strangler Pattern**
       - Bulkhead Pattern
       - **Sidecar Pattern** (service Mesh)
  2. Integration Patterns
       - **API Gateway Pattern** (Auth, Rate Limiting)
       - Aggregator Pattern
       - Proxy Pattern
  3. Database Patterns
       - **Database per Service Pattern**
       - **Shared Database Pattern**
       - **Event Sourcing Pattern**
       - **CQRS Pattern**
       - **Saga Pattern**
  4. Observability Patterns
       - Log Aggregation Pattern
       - Distributed Tracing Pattern
       - Performance Metrics Pattern
       - Health Check API Pattern
  5. Cross-Cutting Concerns Patterns
       - **Externalized Configuration Pattern**
       - **Service Discovery Pattern**
       - **Circuit Breaker Pattern** (Retry / Timeout / Fallback)
       - **Blue-Green Deployment Pattern**
       - **Event-Driven Architecture** (Pub/Sub, Saga Choreography)
