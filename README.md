# ChamTech Software Engineering Portfolio

ChamTech is the personal software engineering portfolio of Deivid Vanegas.

It is presented as a software laboratory and engineering ecosystem, not as a company or commercial organization.

## Portfolio tracks

### Backend Engineering

Projects focused on:

- Java
- Spring Boot
- REST APIs
- PostgreSQL
- Docker
- Automated testing
- API documentation

### Enterprise Integration

Projects focused on:

- MuleSoft
- DataWeave
- API-led connectivity
- ETL and system migration
- Oracle integration
- Error handling
- Observability and process tracking

## Projects

### Cham Orders API

**Status:** Release Candidate

Order management REST API built with Java 21, Spring Boot, PostgreSQL, Flyway, Docker and OpenAPI.

Repository:

https://github.com/Aslannt/cham-orders-api

Verification:

- 38 automated tests
- Clean Maven package
- PostgreSQL 17.10
- Flyway V1 and V2
- Docker Compose
- Complete smoke test
- OpenAPI JSON and YAML
- Standardized 404, 405 and 415 responses

### Cham Orders Integration

**Status:** Planned

MuleSoft integration project that will consume Cham Orders API, transform confirmed orders into a canonical format and simulate delivery to an external system.
