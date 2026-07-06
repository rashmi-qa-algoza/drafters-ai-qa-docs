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
