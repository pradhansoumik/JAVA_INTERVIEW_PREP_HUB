## HLD (High-Level Design)

- Definition
  - What is system design?
  - Designing scalable, reliable distributed systems
  - HLD vs LLD
  - SDLC overview

---

- Components
  - Client
  - Server
  - Load Balancer
  - Web Server
  - Application Server
  - Cache
  - Database

---

- Key Characteristics
  - Scalability
  - Availability
  - Consistency
  - Load Balancing
  - Caching
  - CDN
  - Data Partitioning
  - CAP Theorem
  - Choice of DB
  - Reliability
  - Efficiency
  - Manageability
  - Resiliency

---

- Scalability
  - Definition and real-life examples
  - Horizontal scaling
  - Vertical scaling
  - Auto-scaling

---

- Availability
  - Definition and real-life examples
  - Reliability benchmark (ideally 9s or 11s)

---

- Consistency
  - Definition and real-life examples
  - Strong consistency
  - Eventual consistency

---

- CAP Theorem
  - Consistency, availability, and partition tolerance trade-offs
  - Reasoning behind CAP theorem
  - CP vs AP systems and when to choose each

---

- Load Balancing
  - Definition and examples like Nginx, AWS ELB, Citrix ADC, Google Cloud Load Balancer
  - Placement of load balancers in different layers
  - Benefits of load balancing
  - Smart predictive load balancers
  - Load balancing algorithms
    - Least Connections
    - Least Response
    - Round Robin
    - IP Hashing
    - Least Bandwidth

---

- Caching
  - Definition and principle of caching
  - Real-life examples: Redis, Memcached, Hazelcast
  - Cache hit, cache miss, hit rate, miss rate
  - Cache invalidation
  - Cache write strategies
    - Write-through
    - Write-around
    - Write-back
  - Cache eviction policies
    - FIFO
    - LIFO
    - LRU
    - LFU
    - MRU
  - Cache avalanche

---

- Content Delivery Network (CDN)
  - Serving large amounts of static media
  - Distributed across geographies
  - Performance and latency improvements

---

- Short Polling, Long Polling, WebSocket, and Server-Sent Events
  - Polling technique
  - Short polling / AJAX-based polling
  - Long polling
  - WebSockets for full-duplex communication
  - Server-Sent Events (SSE)

---

- Database, Data Partitioning / Sharding, and Indexing
  - SQL and NoSQL databases
  - MySQL, Postgres, Oracle, MongoDB, Cassandra, etc.
  - Choice of DB and trade-offs
  - Data partitioning
  - Partitioning methods
    - Horizontal / sharding
    - Vertical
    - Directory-based
  - Partitioning criteria
    - Key/hash-based
    - List-based
    - Round-robin
    - Composite/hybrid
  - Problems with partitioning
    - Joins
    - Referential integrity
    - Rebalancing
  - Database indexing
  - Impact of indexing on writes
  - Indexing structures
    - B+ Tree
    - Hash Tables
    - R-Tree
    - Bitmap Index

---

- HLD Template - How to Approach an HLD Interview
  - Requirements clarification
    - Functional
    - Non-functional
    - Extended requirements
  - Back-of-the-envelope calculations
    - Capacity estimation
    - DAU / MAU
  - System API
    - Endpoints and request/response models
  - Defining DB schema
    - Data types and DB selection
  - High-level design
    - Client, server, database, and caching
  - Detailed component-level design
  - Bottlenecks and trade-offs
  - Telemetry and analytics

---

- Case Studies
  - URL Shortener, Pastebin
  - Instagram
  - Twitter
  - WhatsApp
  - Uber
  - Google Drive
  - YouTube
  - Netflix etc.