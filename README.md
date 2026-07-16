# ChamTech Software Engineering Portfolio

ChamTech is the personal software engineering portfolio and software laboratory of **Deivid Vanegas**.

It is not a company or commercial organization. It is an engineering ecosystem created to demonstrate backend development, enterprise integration, API design, automated testing, documentation and local deployment practices.

---

## Portfolio overview

This portfolio combines two complementary engineering tracks:

### Backend Engineering

- Java 21
- Spring Boot
- REST API design
- PostgreSQL
- Flyway
- Docker
- JWT authentication
- Automated testing
- OpenAPI documentation

### Enterprise Integration

- MuleSoft
- Mule Runtime 4
- APIKit
- RAML
- DataWeave
- HTTP integrations
- Pagination
- Correlation tracking
- Canonical data models
- MUnit testing

---

## End-to-end architecture

```mermaid
flowchart LR
    Client[Client / API Consumer]
    Mule[Cham Orders Mule Integration]
    API[Cham Orders API]
    DB[(PostgreSQL 17)]
    File[Canonical JSON / Simulated ERP]

    Client -->|POST /api/v1/order-sync| Mule
    Mule -->|JWT authentication| API
    Mule -->|Paginated CONFIRMED orders| API
    API --> DB
    Mule -->|DataWeave transformation| File
