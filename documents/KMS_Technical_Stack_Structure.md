# KMS Final Technology Stack Specification

> **Notice:** The technologies listed below represent the mandatory and approved technology stack for the Knowledge Management System (KMS) project.

---

## 1. Frontend
- **Framework:** Next.js 15 (App Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS
- **UI Components:** Shadcn UI
- **Data Fetching & State:** TanStack Query (React Query)
- **Form Handling:** React Hook Form
- **Schema Validation:** Zod
- **Icons:** Lucide React

## 2. Backend
- **Runtime Environment:** Node.js
- **Framework:** Express.js
- **Language:** TypeScript
- **API Specification:** REST API
- **API Documentation:** Swagger (OpenAPI)

## 3. Database & ORM
- **Database:** PostgreSQL
- **ORM:** Prisma ORM

## 4. Authentication & Authorization
- **Authentication:** JWT & Refresh Token
- **Authorization:** Role-Based Access Control (RBAC)
- **Password Hashing:** bcrypt

## 5. File Storage
- **Media & File Storage:** ImageKit

## 6. Security
- **Security Headers:** Helmet
- **Origin Control:** CORS
- **Throttling:** Rate Limiting
- **Input Validation:** Zod

## 7. Caching & Logging
- **In-Memory Cache:** Redis
- **Logger:** Pino

## 8. Monitoring & Error Tracking
- **Metrics Collection:** Prometheus
- **Visualization:** Grafana
- **Error Tracking:** Sentry

## 9. Testing
- **Unit & Integration Testing:** Jest
- **API Testing:** Supertest

## 10. DevOps & Infrastructure
- **Containerization:** Docker
- **Reverse Proxy:** Nginx
- **CI/CD Automation:** GitHub Actions
- **Host Environment:** Ubuntu Server / VPS
