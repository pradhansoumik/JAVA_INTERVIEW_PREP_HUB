## Spring Boot Topics

- Spring Boot Fundamentals
  - Spring Framework vs Spring Boot vs Spring Cloud
  - Auto-configuration (@EnableAutoConfiguration, @ConditionalOnClass)
  - Starter dependencies and embedded servers (Tomcat default, Jetty/Undertow alternatives)
  - Spring Boot internals - `@SpringBootApplication` → `@Configuration` + `@EnableAutoConfiguration` + `@ComponentScan`
  - Starter dependencies and embedded servers (Tomcat default, Jetty/Undertow alternatives)
  - Profiles, externalized configuration, YAML vs properties


---

- IoC, DI & Beans
  - IoC container
  - ApplicationContext
  - Dependency Injection → constructor, setter, field (`@Autowired`)
  - Stereotype annotations → `@Component`, `@Service`, `@Repository`, `@Controller`
  - `@Configuration` + `@Bean` vs component scan
  - Bean scopes → singleton, prototype, request, session
  - Bean lifecycle → instantiate, inject, `@PostConstruct`, ready, `@PreDestroy`
  - `@Primary` vs `@Qualifier`
  - Circular dependency → `@Lazy`

---

- Configuration & Profiles
  - `application.properties` vs `.yml`
  - Profiles → `spring.profiles.active`, `@Profile`, `application-dev.yml`
  - `@Value` vs `@ConfigurationProperties`
  - Externalized configuration → env vars, CLI
  - Conditional beans → `@ConditionalOn*`

---

- Web Layer (Spring MVC)
  - `@RestController` vs `@Controller`
  - Request mappings → `@GetMapping`, `@PostMapping`, `@PutMapping`, `@PatchMapping`, `@DeleteMapping`
  - `@PathVariable`, `@RequestParam`, `@RequestBody`
  - DTO layer → Controller ↔ Service (not JPA entities)
  - Validation → `@Valid`, Bean Validation
  - Exception handling → `@ControllerAdvice`, `@ExceptionHandler`, error response structure
  - Filters vs Interceptors
  - Swagger / OpenAPI

---

- Spring Data JPA, Transactions & Hibernate
  - `JpaRepository` / `CrudRepository` → `findById`, `save`, derived queries, `@Query`
  - Entity mapping → `@Entity`, `@Id`, relationships
  - PUT / PATCH with JPA → load entity, map fields, dirty checking, 404 if missing
  - `@Transactional` internals → proxy, self-invocation, rollback, propagation
  - Transaction boundary → service layer
  - Hibernate lazy loading → `LazyInitializationException`, Open Session In View, fetch join / DTO query

---

- Application Architecture
  - Layered design → Controller → Service → Repository → DB
  - Package by layer vs package by feature
  - API contract → DTO → Entity mapping
  - Validation & error model
  - Config per environment (profiles)
  - Health checks → Actuator (`/actuator/health`)

---

- Spring Security (Boot wiring)
  - OAuth2/OpenID Connect flows
  - JWT-based authentication
  - Role-based vs attribute-based access control
  - Security changes in Spring Boot 3 (declarative DSL)
  - Notes: `MICROSERVICE-DESIGN-PATTERNS/00-fundamentals/security/`

---

- Cross-cutting & Ops
  - Actuator → health, info, metrics
  - Logging / MDC
  - `@Async` + executor (not Kafka async)
  - `@Scheduled`
  - AOP → logging / timing
