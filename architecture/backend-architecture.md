# Drafters Backend Architecture

> **Document:** Backend Architecture
>
> **Version:** 1.0
>
> **Owner:** Drafters Engineering & QA Team
>
> **Status:** Active
>
> **Last Updated:** YYYY-MM-DD

---

# Table of Contents

1. Overview
2. Purpose
3. Backend Components
4. Service Architecture
5. API Layer
6. Business Logic Layer
7. Database Layer
8. Third-Party Integrations
9. Authentication & Authorization
10. Background Jobs
11. Logging & Monitoring
12. QA Considerations
13. AI Context
14. Related Documentation
15. Revision History

---

# 1. Overview

The backend is responsible for executing all business logic, processing user requests, managing data, communicating with external services, and exposing secure REST APIs consumed by Web, Android, iOS, and the Admin Portal.

---

# 2. Purpose

This document explains the responsibilities of backend services and how they interact with client applications, databases, and third-party integrations.

---

# 3. Backend Components

Major backend components include:

- Authentication Service
- User Management
- Contest Management
- Draft Service
- Pick'em Service
- Wallet Service
- Payment Service
- Notification Service
- Rankings Service
- Responsible Gaming Service
- Reporting Service
- Admin Services

---

# 4. Service Architecture

```text
Client Applications
        │
        ▼
REST APIs
        │
        ▼
Authentication
        │
        ▼
Business Services
        │
        ▼
Database
        │
        ▼
Third-Party Integrations
```

---

# 5. API Layer

The backend exposes REST APIs for:

- Authentication
- User Profile
- Wallet
- Payments
- Contests
- Draft
- Pick'em
- Rankings
- Notifications

---

# 6. Business Logic Layer

The business layer handles:

- Validation
- Business Rules
- Contest Processing
- Wallet Transactions
- Draft Logic
- Pick'em Logic
- Reward Calculation
- Settlement

---

# 7. Database Layer

Stores:

- Users
- Wallet Transactions
- Contests
- Entries
- Draft Data
- Rankings
- Notifications
- Audit Logs

---

# 8. Third-Party Integrations

Current integrations include:

- Finix
- PayPal
- KYC Provider
- Push Notifications
- Email Services

---

# 9. Authentication & Authorization

Security mechanisms include:

- Authentication
- Session Management
- Role-Based Access Control
- reCAPTCHA
- Admin Portal Two-Factor Authentication

---

# 10. Background Jobs

Examples:

- Contest Settlement
- Leaderboard Updates
- Notifications
- Scheduled Reports
- Cleanup Jobs

---

# 11. Logging & Monitoring

Monitor:

- API Performance
- Errors
- Payment Failures
- Authentication Failures
- Background Jobs

---

# 12. QA Considerations

QA should verify:

- Business Rules
- API Responses
- Database Updates
- Error Handling
- Third-Party Integrations

---

# 13. AI Context

AI agents should use this document to:

- Understand backend processing.
- Generate API tests.
- Analyze business logic.
- Identify service dependencies.
- Generate automation for backend workflows.

---

# 14. Related Documentation

- system-overview.md
- application-architecture.md
- api/
- flows/

---

# 15. Revision History

| Version | Date | Author | Description |
|----------|------|--------|-------------|
| 1.0 | | QA Team | Initial Version |
