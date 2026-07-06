# Drafters AI Agent Guide

This document provides project-specific instructions for AI agents used for QA and automation.

# AGENTS.md

# Drafters AI Agent Operating Manual

## Purpose

This document provides project-specific instructions for AI agents working on the Drafters platform. It serves as the primary knowledge source for AI-assisted development, QA, and automation testing.

The information in this document includes business rules, QA processes, coding standards, testing guidelines, and project-specific workflows that cannot be inferred directly from the source code.

AI agents should always use this document before generating code, test cases, reviewing pull requests, or performing automation-related tasks.

---

# 1. Project Information

## Project Name

Drafters Fantasy Sports Platform

## Project Overview

Drafters is a fantasy sports platform that allows users to create fantasy lineups, participate in contests, draft players, complete Pick'em entries, manage wallets, complete identity verification (KYC), and compete for prizes across multiple sports.

The platform supports Web, Android, iOS, and an Admin Portal used for contest management, user management, payment configuration, reporting, and operational tasks.

## Project Objectives

- Provide a secure fantasy sports platform.
- Support real-money contests.
- Enable multiple fantasy game formats.
- Provide reliable payment processing.
- Maintain fair gameplay.
- Deliver a consistent user experience across all platforms.

## Supported Platforms

- Web
- Android
- iOS
- Admin Portal

## Target Users

### End Users

- Fantasy Sports Players

### Internal Users

- QA Engineers
- Developers
- Product Managers
- Customer Support
- Operations Team
- Administrators

## Major Functional Areas

- User Registration
- Authentication
- Profile Management
- Identity Verification (KYC)
- Wallet
- Payments
- Contest Management
- Draft
- Pick'em
- Props
- Rankings
- Leaderboards
- Notifications
- Responsible Gaming
- Promotions
- Admin Portal

## Technology Stack

### Frontend

- Angular (Web)

### Mobile

- Android-kotlin
- iOS-swift

### Backend

- NestJS
- nodeJS
- php

### Database

- MongoDB
- mysql

### Cache

- Redis

### Cloud

- AWS

## AI Agent Scope

This repository is intended to support AI-assisted:

- Manual QA
- Test Case Generation
- Playwright automation
- Appium Automation
- API Test Generation
- Regression Analysis
- Pull Request Review
- Bug Analysis
- Documentation
- Automation Maintenance

The AI agent must always follow the documented business rules and QA standards contained in this repository.


# 2. Repository Structure

## Overview

This repository serves as the central knowledge base for AI-assisted QA, test automation, and project documentation for the Drafters platform.

The repository is organized to help AI agents quickly locate project documentation, business rules, feature flows, testing standards, and automation guidelines.

```
drafters-ai-qa-docs/
│
├── README.md
├── AGENTS.md
│
├── flows/
├── automation/
├── api/
├── test-data/
└── reports/
```

---

## Directory Details

### AGENTS.md

The primary instruction document for AI agents.

Contains:

- Project overview
- Business rules
- QA guidelines
- Coding standards
- Deployment workflow
- AI responsibilities
- Safety rules
- Reporting standards

AI agents should always read this document before generating code, automation scripts, or QA reports.

---

### flows/

Contains feature-wise documentation.

Each module should have its own Markdown file describing:

- Feature overview
- User journey
- Business rules
- Test scenarios
- Expected behavior
- Edge cases
- Validation points
- Automation considerations

Examples:

```
flows/
├── authentication.md
├── registration.md
├── login.md
├── kyc.md
├── wallet.md
├── finix-payment.md
├── contest.md
├── draft.md
├── pickem.md
├── props-booster.md
├── ranking.md
├── responsible-gaming.md
├── notifications.md
└── profile.md
```

---

### automation/

Contains automation standards and implementation guidelines.

Examples include:

- Appium framework standards
- Page Object Model (POM) guidelines
- Locator strategy
- Coding standards
- Naming conventions
- Reusable utilities

---

### api/

Contains API-related documentation.

Each API document should include:

- Endpoint information
- Request parameters
- Response structure
- Validation rules
- Error handling
- Authentication requirements

---

### test-data/

Contains testing resources such as:

- Test accounts
- Sample datasets
- Test scenarios
- Environment-specific test configurations

No production credentials or sensitive information should be stored in this directory.

# 3. Development Environment

## Overview

The Drafters platform consists of Web, Android, iOS, Backend, and Admin Portal applications.

QA testing is primarily performed using dedicated staging environments. Local development setup is typically used by the development team, while QA validates features using deployed staging builds and production build.

---

## Web Application

Environment:
- Staging
- Production

QA Activities:
- Functional Testing
- Regression Testing
- Cross-browser Testing
- UI/UX Validation
- API Verification
- Console Log Verification

---

## Android Application

Build Distribution:
- Staging APK
- production APK

QA Activities:
- Functional Testing
- Regression Testing
- UI Validation
- Deep Link Testing
- Push Notification Testing
- Payment Flow Validation

---

## iOS Application

Build Distribution:
- Staging IPA
- TestFlight (production)

QA Activities:
- Functional Testing
- Regression Testing
- User Journey Validation
- Payment Flow Validation
- Push Notification Testing
- Email Journey Verification

---

## Admin Portal

Environment:
- Staging

QA Activities:
- Feature Configuration
- Contest Management
- Payment Configuration
- Responsible Gaming Configuration
- User Management
- Reporting Validation

---

## Backend Services

Backend services are deployed to staging environments and are validated through:

- API Testing
- Database Verification
- Log Analysis
- Integration Testing

---

## AI Agent Instructions

AI agents should assume that testing is performed against the latest available staging environment unless explicitly instructed otherwise.

Do not assume that local development environments are available.

Always reference the appropriate environment before generating test cases or automation scripts.

Never perform destructive operations against production environments.

# 4. Environment URLs

## Overview

The Drafters platform is deployed across multiple environments. Actual URLs are managed securely and should not be stored in this repository.

AI agents should use the appropriate environment provided by the QA or development team.

---

## Development Environment

| Component | URL |
|-----------|-----|
| Web | `<DEV_WEB_URL>` |
| Backend API | `<DEV_API_URL>` |
| Admin Portal | `<DEV_ADMIN_URL>` |

---

## Staging Environment

| Component | URL |
|-----------|-----|
| Web | `<STAGING_WEB_URL>` |
| Backend API | `<STAGING_API_URL>` |
| Admin Portal | `<STAGING_ADMIN_URL>` |
| Android | `<STAGING_ANDROID_BUILD>` |
| iOS | `<TESTFLIGHT_STAGING_BUILD>` |

---

## Production Environment (Reference Only)

| Component | URL |
|-----------|-----|
| Web | `<PRODUCTION_WEB_URL>` |
| Backend API | `<PRODUCTION_API_URL>` |
| Admin Portal | `<PRODUCTION_ADMIN_URL>` |

---

## Security Guidelines

- Never store production URLs, credentials, or API keys directly in this repository.
- Environment-specific values should be obtained from the organization's secure configuration or secret management system.
- AI agents must never perform destructive operations against production environments.

---

### reports/

Contains QA reporting templates.

Examples:

- Test execution reports
- Regression reports
- AI-generated QA reports
- Bug summary templates
- Automation execution reports

---

## AI Agent Navigation

When performing tasks, AI agents should use the repository in the following order:

1. Read `AGENTS.md` to understand the project context and standards.
2. Read the relevant file under `flows/` to understand the specific feature.
3. Refer to `api/` when API behavior or validation is required.
4. Follow `automation/` guidelines when generating or reviewing automation code.
5. Use `test-data/` for valid test inputs.
6. Generate outputs using the templates available in `reports/`.

## Documentation Maintenance

- Keep documentation up to date with every feature enhancement or business rule change.
- Create a new module document whenever a new feature is introduced.
- Remove obsolete documentation after feature deprecation.
- Ensure all documentation remains synchronized with the latest application behavior.
