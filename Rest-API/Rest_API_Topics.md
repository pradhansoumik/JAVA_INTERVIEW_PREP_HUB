## Rest API Topics

- REST Fundamentals:

  - Stateful vs stateless REST API
  - REST Principles → HATEOAS, Idempotency, Partial Update, Validation
  - API contract → Request/response modeling",
  - Idempotency & safe methods

---

- REST API Design Principles:

  - Resource naming & URI design → ✅ Good: GET /users/123, ❌ Bad: GET /getUserById?id=123
  - HTTP methods → GET, POST, PUT, PATCH, DELETE
  - HTTP status codes → 2xx, 3xx, 4xx, 5xx
  - Versioning strategies → /api/v1/users
  - Pagination, filtering & sorting
  - Error handling/Error response structure → Return structured error objects with codes and messages
  - Security
  - Monitoring & Logging

---

- Security & Authentication:

  - Authentication vs authorization
  - JWT, OAuth 2.0 basics
  - API keys & token-based auth
  - Role-based access control
  - HTTPS & secure headers

---

- Documentation & Best Practices:

  - Swagger / OpenAPI
  - DTO layer — Controller ↔ Service boundaries
  - Rate limiting & throttling
  - HATEOAS basics
  - API testing — Postman, contract testing
