## Microservices Topics

- Monolithic vs Microservices Architecture
- Characteristics of Microservices
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
       - Database per Service Pattern
       - Shared Database Pattern
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