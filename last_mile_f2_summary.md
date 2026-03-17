
# “Last-Mile” Challenge: *Satisfies F2:A-F*

**ODOS 3.1 RFQ (70SBUR26Q00000001)**  
Factor 2 – Coding Challenge | Section 4.3 Evaluation Criteria

---

# Evaluation Coverage

## 1. Code Quality — **STRONG**

- Java 21, Spring Boot 3.5.11, React 18, TypeScript 5.7
- Spotless (Java) + ESLint v9 + Husky **pre-commit hooks**
- SonarQube integrated with CI pipeline (**88%+ coverage gates**)
- **JaCoCo at 85% minimum threshold** enforced on builds
- OWASP DependencyCheck + Grype container image scanning
- Multi-stage Docker builds (JDK 21 builder + JRE-alpine runtime)
- `build-all-services.sh`, `run-all-services.sh`, Maven wrapper

---

## 2. API Integration — **STRONG**

- RESTful APIs via Spring WebMVC/WebFlux across all services
- SpringDoc OpenAPI with **auto-generated Swagger UI (v2.7.0)**
- OpenAPI-typescript generates **type-safe frontend clients**
- **Kong API Gateway** (DB-less) for routing, rate limiting, auth plugins
- Inter-service communication via **WebClient + Kafka async messaging**

---

## 3. Microservices — **STRONG**

- **7+ independent services:** user, permitflow, notification, form, etc.
- Each service has its own Dockerfile, Helm chart, and CI/CD pipeline
- Shared PostgreSQL with **per-service schemas**
- `alpha-omega-cc-common` shared library for cross-cutting concerns
- **Linkerd service mesh with mTLS** between all services
- **Kubernetes (EKS)** orchestration with HPA auto-scaling

---

## 4. DevOps and CI/CD — **STRONG**

- GitHub Actions CI with **smart change detection** (`ci.yml`)
- **ArgoCD GitOps** for continuous deployment to EKS
- Terraform IaC with **10 layered modules** (bootstrap → tools-config)
- Multi-environment: **dev, staging, production** with per-env configs
- ECR (private) for container images, Nexus for Maven artifacts
- Reusable workflows: `shared-java-build.yml`, `shared-frontend-build.yml`
- **Smoke tests post-deploy** (functional + accessibility)

---

## 5. User-Centric Design — **STRONG**

- **USWDS 3.13.0** (US Web Design System) component library
- `@common/react-design-framework` with **Storybook (port 6006)**
- Responsive design via **USWDS + SASS styling**
- Accessibility: ARIA labels, focus management, `focus-trap-react`
- User-facing app: registration, permit application, status tracking
- Admin dashboard: user management, review, assignment
- React Hook Form 7.68 with validation, dark/light mode
- **1-day Design Sprint** with persona definition and usability testing

---

## 6. Testing — **STRONG**

### Backend
- JUnit 5 + Spock/Groovy BDD (`src/test/groovy/`)
- Gherkin/Cucumber feature files via `cucumber-java`

### Frontend
- Vitest 4.0.16 + Testing Library

### End-to-End
- Playwright 1.49.1 (Chromium, Firefox, WebKit)

### Accessibility
- `axe-core` 4.10.2
- `@axe-core/playwright`
- Storybook a11y

### Quality Gates
- **JaCoCo ≥ 85% or build fails**

### Integration
- TestContainers (PostgreSQL) + H2 in-memory

### Role-based testing
- `@applicant`, `@coordinator`, `@reviewer`, `@admin`

---

## 7. Authentication and Authorization (RBAC) — **STRONG**

- AWS Cognito (OAuth2/OIDC) + mock auth service for local dev
- JWT tokens: RS256 via JWKS, OAuth2 Resource Server pattern
- Role-based access:
  - `@PreAuthorize` (API)
  - `<RequireRole>` (UI)
- Roles: Applicant, Coordinator, Reviewer, Admin
- Secure token refresh in **httpOnly cookie (XSS protection)**
- Spring Security 6.5.4 with per-endpoint authorization

---

## 8. Reporting and Dashboarding — **STRONG**

- React Google Charts 5.2.1
- TanStack React Table 8.21.3
- Admin dashboard metrics and trends
- Monitoring: **Prometheus + Grafana**
- Cost monitoring: **Kubecost / OpenCost**

---

# Exceeding Requirements

## User-Centered Design
USWDS + Storybook + Design Sprint + Persona Research

## DevSecOps Pipeline
7 automated quality gates with **shift-left security**

## Accessibility (Section 508)
WCAG 2.1 AA + automated **axe-core testing**

## Service Mesh (Linkerd mTLS)
Zero-trust networking beyond typical challenge scope

---

# USCIS Tech Landscape Alignment

## PASS
Java 21 • React 18 • PostgreSQL • GitHub Actions • Docker • EKS  
Terraform • ArgoCD • Helm 3.x • Prometheus/Grafana • Vault  
SonarQube • Nexus • NGINX • Linkerd • Node.js • Maven • Liquibase

## NOTE
Cognito (AWS Serverless)  
Playwright (modern Selenium alternative)  
GitHub Actions (also used alongside Jenkins in USCIS environments)

## PASS
Cucumber/Gherkin feature files alongside Spock BDD

---

# Summary Scorecard

| Area | Result |
|-----|------|
| Code Quality | **STRONG** |
| API Integration | **STRONG** |
| Microservices | **STRONG** |
| DevOps CI/CD | **STRONG** |
| User-Centric Design | **STRONG** |
| Testing | **STRONG** |
| Auth/RBAC | **STRONG** |
| Reporting | **STRONG** |

---

# Overall Confidence

**8 / 8 STRONG**  
All criteria **met or exceeded**.
