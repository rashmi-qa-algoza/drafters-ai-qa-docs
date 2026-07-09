# Drafters System Overview

> **Document:** System Overview
>
> **Version:** 1.0
>
> **Owner:** Drafters Engineering & QA Team
>
> **Status:** Active
>
> **Platforms:** Web | Android | iOS | Admin Portal
>
> **Last Updated:** YYYY-MM-DD

---

# Table of Contents

1. Overview
2. Purpose
3. Platform Overview
4. Target Users
5. High-Level System Architecture
6. Core Business Modules
7. Platform Components
8. Third-Party Integrations
9. High-Level User Journey
10. Data Flow Overview
11. Environment Overview
12. Security Overview
13. Technology Stack
14. Related Documentation
15. Revision History

---

# 1. Overview

## Description

Drafters is a multi-platform Fantasy Sports application that enables users to participate in fantasy contests, manage their wallets, complete identity verification, join drafts, play Pick'em contests, and compete in leaderboard-based competitions.

The platform is available on:

- Web
- Android
- iOS

and is supported by an Admin Portal used for operational and business management.

---

# 2. Purpose

The purpose of this document is to provide a high-level understanding of the Drafters platform architecture.

This document serves as the entry point for:

- QA Engineers
- Developers
- Product Managers
- Business Analysts
- Automation Engineers
- AI Agents

Readers should review this document before studying individual feature documentation.

---

# 3. Platform Overview

The Drafters ecosystem consists of multiple applications working together.

```

                         Drafters Platform

      ┌───────────────┬───────────────┬───────────────┐
      │               │               │
      ▼               ▼               ▼
   Web App      Android App      iOS App
      │               │               │
      └───────────────┼───────────────┘
                      ▼
                Backend APIs
                      │
      ┌───────────────┼─────────────────────┐
      │               │                     │
      ▼               ▼                     ▼
 Authentication   Contest Engine      Payment Services
      │               │                     │
      └───────────────┼─────────────────────┘
                      ▼
                  Database
                      │
      ┌───────────────┼────────────────────┐
      ▼               ▼                    ▼
 Notification     KYC Service       Analytics

```

---

# 4. Target Users

The platform supports multiple user types.

| User Type | Description |
|------------|-------------|
| End User | Participates in fantasy sports contests |
| Administrator | Configures contests, promotions, and platform settings |
| QA Engineer | Validates application functionality |
| Developer | Builds and maintains platform features |
| Product Manager | Defines business requirements |
| Support Team | Assists users with platform-related issues |

---

# 5. High-Level System Architecture

The Drafters platform consists of the following major layers:

## Client Applications

- Web Application
- Android Application
- iOS Application

## Backend Services

- Authentication
- User Management
- Contest Management
- Wallet
- Payments
- Notifications
- Responsible Gaming
- Rankings

## Data Layer

- Database
- Cache
- Logs
- Analytics

## External Services

- Payment Providers
- Identity Verification
- Push Notifications
- Email Services

---

# 6. Core Business Modules

The platform includes the following primary business modules.

### User Management

- Authentication
- Registration
- Login
- Profile
- Session Management

### Verification

- KYC
- Responsible Gaming

### Wallet & Payments

- Wallet
- Finix
- PayPal

### Fantasy Sports

- Lobby
- Contest
- Draft
- Slow Draft
- Fast Draft
- Best Ball
- Best Ball Survival

### Pick'em

- Pick'em
- Props
- Props Booster

### Engagement

- Rankings
- Leaderboards
- Notifications
- Rewards

### Administration

- Admin Portal
- Contest Configuration
- User Management
- Reporting

---

# 7. Platform Components

The Drafters platform is composed of:

- Web Client
- Android Client
- iOS Client
- Backend APIs
- Admin Portal
- Database
- Third-party Integrations
- Monitoring & Logging

Each component plays a specific role within the platform and interacts with other components through secure APIs.

---

# 8. Third-Party Integrations

The platform integrates with several external services.

Examples include:

- Finix Payment Gateway
- PayPal
- KYC Verification Provider
- Push Notification Services
- Email Services
- Analytics & Monitoring Services

These integrations extend the platform's functionality while maintaining a consistent user experience.

---

# 9. High-Level User Journey

A typical user journey is illustrated below.

```

Registration

↓

Authentication

↓

KYC Verification

↓

Wallet Funding

↓

Browse Lobby

↓

Join Contest

↓

Participate in Draft / Pick'em

↓

Contest Settlement

↓

Leaderboard & Rewards

```

---

# 10. Data Flow Overview

```

User

↓

Web / Android / iOS

↓

Backend API

↓

Business Services

↓

Database

↓

Third-party Services

↓

Response to User

```

All communication between client applications and backend services occurs through secure APIs.

---

# 11. Environment Overview

The Drafters platform is deployed across multiple environments.

| Environment | Purpose |
|------------|---------|
| Development | Feature development and initial validation |
| Staging | QA testing and business validation |
| Production | Live environment for end users |

Production should only be used for smoke testing and production verification.

---

# 12. Security Overview

The platform includes several security mechanisms to protect user accounts and data.

Examples include:

- Authentication
- Session Management
- HTTPS Communication
- reCAPTCHA Protection
- Two-Factor Authentication (Admin Portal)
- Secure Payment Processing
- Role-Based Access Control

---

# 13. Technology Stack

The platform consists of multiple technologies.

## Client Applications

- Web
- Android
- iOS

## Backend

- REST APIs
- Authentication Services
- Business Services

## External Integrations

- Finix
- PayPal
- KYC Provider
- Push Notification Services

> **Note:** This section should be updated as the technology stack evolves.

---

# 14. Related Documentation

- AGENTS.md
- README.md
- application-architecture.md
- frontend-architecture.md
- backend-architecture.md
- mobile-architecture.md
- deployment-flow.md
- flows/
- api/

---

# 15. Revision History

| Version | Date | Author | Description |
|----------|------|--------|-------------|
| 1.0 | YYYY-MM-DD | QA Team | Initial Version |
