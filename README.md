Hi, I'm Ethan

Backend software engineer based in the Midwest. I build production Java services with Spring Boot, with a background in event-driven systems (Kafka), PostgreSQL, and observability tooling from three years at a Fortune 500 financial services client.

Currently building distributed systems end-to-end — most recently a ticket-reservation platform with a Kafka payment saga and Redis distributed locking, deployed on AWS — and looking for my next backend or full-stack role.

Stack I work in: Java 21 · Spring Boot · Spring Security · JPA · Apache Kafka · Redis (Redisson) · PostgreSQL · Flyway · Testcontainers · Docker · AWS (ECS Fargate, RDS, ElastiCache, CloudFront) · React · TypeScript

Pinned projects:

**ticket-reservation** — A distributed event-ticket reservation system. Zero double-sell under concurrent load via a three-layer defense (Redis TTL holds with Redisson locks, JPA optimistic locking, partial-unique-index backstop). Payment flow is a Kafka saga: transactional outbox, idempotent consumers with dedup tables, timeout compensation — with end-to-end Testcontainers suites proving at-least-once semantics (crash-replay, duplicate delivery, out-of-order events). Deployed on AWS: two ECS Fargate instances behind an ALB and CloudFront, RDS Postgres, ElastiCache, self-managed Kafka on EC2, secrets via SSM. React + TypeScript frontend.

**kitchen** — A full-stack inventory app. Spring Boot backend with JWT auth, refresh token rotation, rate limiting, and Testcontainers integration tests. React + TypeScript frontend with custom tags per user and autocomplete from previous entries.

ethaniluong@gmail.com · LinkedIn
