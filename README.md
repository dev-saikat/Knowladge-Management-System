# Knowledge Management System (KMS)

An enterprise-grade, high-performance platform engineered for organization-wide knowledge sharing, structured documentation, role-based collaboration, and centralized learning assets.

---

## Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Team Structure & Leadership](#team-structure--leadership)
- [Approved Technology Stack](#approved-technology-stack)
- [Team Development & GitHub Workflow](#team-development--github-workflow)
- [Development & Contribution Guidelines](#development--contribution-guidelines)
- [License](#license)

---

## Overview

The **Knowledge Management System (KMS)** is designed to streamline knowledge capture, content organization, and team collaboration. Built on a modern decoupled architecture using **Next.js 15** and **Node.js with Express.js**, the platform delivers fast performance, strict type safety, role-based security, and real-time observability.

---

## Key Features

- **Decoupled Architecture:** High-performance Next.js 15 client paired with a lightweight Node.js/Express REST API backend.
- **Role-Based Access Control (RBAC):** Granular permissions for Administrators, Content Creators, and Standard Users.
- **Secure Authentication:** JWT Access Tokens with HTTP-only Refresh Token rotation and Redis-backed session control.
- **Type-Safe Data Engine:** PostgreSQL database managed via Prisma ORM for end-to-end type safety.
- **Cloud Asset Delivery:** Direct signed media uploads and automated image optimization via ImageKit CDN.
- **Production Observability:** Centralized logging with Pino, exception tracking via Sentry, and metric harvesting via Prometheus and Grafana.

---

## Team Structure & Leadership

### Project Leadership
- **Aditya Halder** — Team Lead (Frontend & Database Design)
- **Saikat Bera** — Team Lead (Backend & DevOps)

### Core Development Team
- Mahek Sultana
- Darshil Raj
- Sulagna Bose
- Sourindra Mohan Das
- Bhumika Sethi
- Sreyasi
- Ankita Chatterjee
- Sohan Moyra
- Sawstika Das
- Suraj SK

---

## Approved Technology Stack

The project strictly enforces the following mandatory technology stack:

### Frontend Tier
- **Framework:** Next.js 15 (App Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS
- **UI Components:** Shadcn UI
- **Data Fetching & State:** TanStack Query (React Query v5)
- **Form Management:** React Hook Form
- **Schema Validation:** Zod
- **Icons:** Lucide React

### Backend Tier
- **Runtime Environment:** Node.js
- **Framework:** Express.js
- **Language:** TypeScript
- **API Protocol:** REST API
- **API Documentation:** Swagger (OpenAPI 3.0)

### Database & Storage
- **Database:** PostgreSQL
- **ORM:** Prisma ORM
- **Media Storage & CDN:** ImageKit

### Authentication & Security
- **Authentication:** JWT & Refresh Tokens
- **Access Control:** Role-Based Access Control (RBAC)
- **Password Encryption:** bcrypt
- **Security Suite:** Helmet, CORS, Rate Limiting, Zod Validation

### Caching, Logging & Observability
- **In-Memory Cache:** Redis
- **Logging:** Pino Logger
- **Metrics & Visualization:** Prometheus & Grafana
- **Error Tracking:** Sentry

### Testing & Quality Assurance
- **Unit & Integration Testing:** Jest
- **API Endpoint Testing:** Supertest

### DevOps & Infrastructure
- **Containerization:** Docker & Docker Compose
- **Reverse Proxy:** Nginx
- **CI/CD Pipeline:** GitHub Actions
- **Host Server OS:** Ubuntu Server / VPS

---

## Team Development & GitHub Workflow

All team members must follow this standardized Git & GitHub workflow for code contributions.

### Prerequisites

Ensure you have Git installed and configured on your system.

---

### Step 1: Fork the Main Repository

1. Open the main project repository on GitHub: `https://github.com/dev-saikat/Knowladge-Management-System`
2. Click the **Fork** button (top-right corner) to create a copy under your personal GitHub account.

---

### Step 2: Clone Your Forked Repository

Open your terminal or command prompt and clone your personal fork to your local machine:

```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/Knowladge-Management-System.git
cd Knowladge-Management-System
```

---

### Step 3: Connect Local Repository to Main (Upstream) Remote

Add the main repository as an `upstream` remote to easily pull updates made by team members:

```bash
git remote add upstream https://github.com/dev-saikat/Knowladge-Management-System.git
git fetch upstream
```

Verify your remote connections:
```bash
git remote -v
# Output should show 'origin' (your fork) and 'upstream' (main repo)
```

---

### Step 4: Create a Dedicated Feature Branch

Always create a new branch named strictly after your name (e.g. `feature/xyz`):

```bash
# Pattern: feature/xyz (where xyz is your name)
git checkout -b feature/xyz
```

---

### Step 5: Commit and Push Your Changes

After making changes and verifying them locally:

1. **Check Modified Files:**
   ```bash
   git status
   ```

2. **Stage and Commit Changes:**
   ```bash
   git add .
   git commit -m "feat: update project codebase"
   ```

3. **Push to Your Personal Fork:**
   ```bash
   git push -u origin feature/xyz
   ```

---

### Step 6: Create a Pull Request (PR)

1. Go to your personal repository fork on GitHub.
2. Click the **Compare & pull request** button next to your recently pushed branch.
3. Verify the PR settings:
   - **Base Repository:** `dev-saikat/Knowladge-Management-System` (Branch: `main`)
   - **Head Repository:** `YOUR_USERNAME/Knowladge-Management-System` (Branch: `feature/xyz`)
4. Write a clear title and summary of changes.
5. Request review from Team Leads (**Aditya Halder** / **Saikat Bera**).

---

### Step 7: Keep Your Fork Updated (Syncing with Main)

Before starting new work or submitting a PR, update your local branch with the latest changes from the main repo:

```bash
git checkout main
git pull upstream main
git push origin main
```

---

## Development & Contribution Guidelines

1. **Branch Naming Rule:**
   - Always create branches using the pattern `feature/xyz` (where `xyz` is your name).

2. **Commit Conventions:**
   - `feat: ...` for new features
   - `fix: ...` for bug fixes
   - `docs: ...` for documentation updates
   - `refactor: ...` for code refactoring

3. **Code Review Rule:**
   - Direct pushes to the `main` branch are restricted.
   - Every Pull Request requires approval from at least one **Team Lead** (`Aditya Halder` or `Saikat Bera`) before merging.

---

## License

This project is proprietary and maintained by the **KMS Development Team**. All rights reserved.