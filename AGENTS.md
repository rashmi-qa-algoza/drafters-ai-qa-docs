# Drafters AI Operating Manual

Repository: drafters-ai-qa-docs

Owner: Drafters QA Team

Last Updated: 2026-07-08

Status: Active

# 1. Purpose

## Overview

The **Drafters AI Documentation Repository** serves as the official knowledge base for AI-assisted software testing, quality assurance, automation, and project documentation for the Drafters Fantasy Sports Platform.

This repository is designed to provide a single source of truth for business workflows, application behavior, QA standards, automation guidelines, and technical documentation.

It enables AI tools and engineering teams to understand the Drafters platform consistently without relying on undocumented knowledge or individual team members.

---

## Objectives

The primary objectives of this repository are to:

- Centralize project knowledge.
- Standardize QA and automation practices.
- Document business rules and workflows.
- Reduce onboarding time for new team members.
- Improve collaboration between QA, Developers, Product Managers, and Business Analysts.
- Enable AI-assisted development and testing.
- Maintain accurate and version-controlled documentation.

---

## Intended Audience

This repository is intended for:

- QA Engineers
- Automation Engineers
- Software Developers
- Product Managers
- Business Analysts
- Support Engineers
- New Team Members
- AI Assistants (ChatGPT, Cursor, Claude Code, GitHub Copilot, etc.)

---

## Repository Goals

This repository should enable users and AI agents to understand:

- How the Drafters platform works.
- Business workflows.
- Feature behavior.
- QA processes.
- Automation standards.
- API expectations.
- Project architecture.
- Deployment workflow.
- Reporting standards.

---

## AI Usage

AI agents should use this repository before performing tasks such as:

- Generating manual test cases.
- Creating Appium automation.
- Generating Playwright or Cypress automation.
- Creating API test cases.
- Reviewing pull requests.
- Performing regression analysis.
- Investigating defects.
- Generating QA reports.
- Creating technical documentation.

AI agents must always follow the documented business rules and project standards.

---

## Repository Principles

This repository follows the following principles:

- Documentation should always reflect the latest application behavior.
- Business rules take priority over implementation assumptions.
- Documentation should be clear, concise, and maintainable.
- Every feature should have dedicated documentation.
- AI should never assume undocumented functionality.
- Documentation changes should be version controlled.

---

## Scope

This repository documents the complete Drafters platform, including:

- Web Application
- Android Application
- iOS Application
- Admin Portal
- APIs
- Business Workflows
- QA Standards
- Automation Guidelines
- Release Processes

---

## Out of Scope

This repository does not store:

- Production credentials
- API secrets
- Environment secrets
- Sensitive customer information
- Internal confidential data
- Production database information

Sensitive information must always be managed using approved secure systems.

---

## Success Criteria

This repository is considered successful when:

- A new team member can understand the Drafters platform without relying on verbal explanations.
- AI agents can generate accurate and consistent outputs.
- Documentation remains synchronized with product changes.
- QA and Development teams follow the same documented standards.
- Business knowledge is preserved and easily accessible.

# 2. AI Workflow

## Overview

This repository is designed to guide AI agents through a structured workflow before generating code, automation scripts, test cases, documentation, or QA reports.

AI agents should never make assumptions about the Drafters platform. Instead, they should follow the documented workflow and use this repository as the primary source of project knowledge.

---

## Standard AI Workflow

Every AI task should follow the workflow below:

```
Start
   │
   ▼
Read README.md
   │
   ▼
Read AGENTS.md
   │
   ▼
Identify the feature or business domain
   │
   ▼
Read the corresponding document in the flows/ directory
   │
   ▼
Review related API documentation (if applicable)
   │
   ▼
Review automation guidelines (if applicable)
   │
   ▼
Generate the requested output
   │
   ▼
Validate output against documented business rules
   │
   ▼
Generate final report or response
```

---

## AI Decision Process

Before performing any task, AI agents should answer the following questions:

1. Which feature or module is being requested?
2. Which business rules apply?
3. Which platforms are affected (Web, Android, iOS, Admin)?
4. Are there related APIs that should be considered?
5. Are there existing automation standards?
6. Are there known limitations that affect this task?

---

## AI Repository Navigation

AI agents should use the repository in the following order:

### Step 1

Read:

- README.md

Purpose:

Understand the repository structure and available documentation.

---

### Step 2

Read:

- AGENTS.md

Purpose:

Understand project standards, QA guidelines, business rules, AI responsibilities, and safety requirements.

---

### Step 3

Read:

- architecture/

Purpose:

Understand how the Drafters platform is organized and how different components interact.

---

### Step 4

Read:

- flows/

Purpose:

Understand the complete feature workflow, business logic, validations, and user journey.

---

### Step 5

Read:

- api/

Purpose:

Understand API behavior, request/response expectations, and validation rules.

---

### Step 6

Read:

- automation/

Purpose:

Follow project automation standards, coding guidelines, and best practices.

---

### Step 7

Read:

- test-data/

Purpose:

Use approved test accounts, sample data, and environment-specific information.

---

### Step 8

Read:

- troubleshooting/

Purpose:

Check known issues, common failures, and recommended resolutions before reporting defects.

---

### Step 9

Generate Output

AI agents may generate:

- Manual Test Cases
- Regression Test Cases
- API Test Cases
- Appium Automation
- Playwright Automation
- QA Reports
- Bug Analysis
- Pull Request Reviews
- Documentation Updates

---

## AI Validation Checklist

Before returning a response, AI agents should verify:

- Business rules have been followed.
- Platform-specific behavior has been considered.
- Related documentation has been reviewed.
- Automation follows project standards.
- No undocumented assumptions have been made.
- Sensitive information is not exposed.

---

## AI Principles

AI agents should always:

- Use documented business rules.
- Generate reusable outputs.
- Follow QA best practices.
- Follow coding standards.
- Request clarification when documentation is incomplete.
- Explain assumptions when necessary.

AI agents should never:

- Invent business logic.
- Ignore documented workflows.
- Bypass safety rules.
- Generate destructive operations.
- Use production credentials.

---

## Related Documentation

- README.md
- architecture/
- flows/
- api/
- automation/
- test-data/
- troubleshooting/

# 3. Project Information

## Overview

Drafters is a fantasy sports platform that enables users to participate in multiple fantasy sports contests through Web, Android, and iOS applications. The platform provides various game formats, secure payment processing, identity verification, contest management, and administrative tools.

This repository documents the functional behavior, business workflows, QA standards, automation guidelines, and AI instructions for the Drafters platform.

---

## Project Objectives

The primary objectives of the Drafters platform are:

- Deliver a secure fantasy sports experience.
- Support multiple fantasy contest formats.
- Provide reliable payment processing.
- Ensure regulatory compliance through KYC and Responsible Gaming.
- Maintain consistent functionality across Web, Android, and iOS.
- Deliver scalable and maintainable software through standardized engineering practices.

---

## Supported Platforms

The Drafters platform consists of the following applications:

### Web Application

Allows users to:

- Register and log in
- Join contests
- Draft players
- Participate in Pick'em
- Manage wallet
- View rankings
- Manage profile

---

### Android Application

Provides the complete fantasy sports experience optimized for Android devices.

---

### iOS Application

Provides the complete fantasy sports experience optimized for iPhone and iPad devices.

---

### Admin Portal

Used by internal teams to manage:

- Users
- Contests
- Promotions
- Payments
- Responsible Gaming
- Reports
- Feature configurations

---

## Major Business Modules

The platform includes the following major business domains:

- Authentication
- Registration
- User Profile
- Identity Verification (KYC)
- Wallet
- Payments
- Contest Lobby
- Draft
- Pick'em
- Props
- Props Booster
- Best Ball
- Best Ball Survival
- Rankings
- Leaderboards
- Rewards
- Notifications
- Responsible Gaming
- Admin Portal

Each business domain has dedicated documentation under the `flows/` directory.

---

## Primary Users

The platform supports different types of users.

### End Users

Fantasy sports players using Web, Android, or iOS applications.

### Internal Users

- QA Engineers
- Software Developers
- Product Managers
- Business Analysts
- Customer Support
- Operations Team
- Administrators

---

## Technology Stack

> **Note:** Update this section to match the actual technologies used by the project.

### Frontend

- Angular (Web)

### Mobile

- Android: Kotlin+JAVA
- iOS: Swift

### Backend

- NestJS
- NodeJS
- PHP

### Database

- MongoDB
- mysql

### Cache

- Redis

### Cloud Infrastructure

- AWS

### Third-Party Integrations

- Payment Gateway
- KYC Provider
- Push Notification Service
- Email Service

---

## Repository Scope

This repository documents:

- Business workflows
- Feature documentation
- User journeys
- QA standards
- API guidelines
- Automation standards
- Test data
- Troubleshooting guides
- Release documentation
- AI operating guidelines

---

## Related Documentation

- `README.md`
- `architecture/system-overview.md`
- `architecture/application-architecture.md`
- `flows/`
- `api/`

# 4. Repository Structure

## Overview

The **Drafters AI Documentation Repository** is organized to provide a structured and centralized knowledge base for the Drafters platform.

Each directory has a specific purpose and should be maintained independently. AI agents and team members should navigate the repository using the documented folder structure to locate relevant information.

The repository is designed to support:

- Business Documentation
- QA Documentation
- AI-Assisted Development
- Automation Testing
- API Documentation
- Release Documentation
- Team Knowledge Sharing

---

## Repository Structure

```
drafters-ai-qa-docs/
│
├── README.md
├── AGENTS.md
│
├── architecture/
├── flows/
├── api/
├── automation/
├── test-data/
├── reports/
├── troubleshooting/
└── release-notes/
```

---

# README.md

## Purpose

Provides an introduction to the repository.

Contents include:

- Repository overview
- Folder structure
- Getting started guide
- Documentation standards
- Contribution guidelines

---

# AGENTS.md

## Purpose

The primary instruction document for AI agents.

Contains:

- Project standards
- AI workflow
- Business domains
- QA standards
- Coding standards
- Deployment workflow
- Safety rules
- Reporting guidelines

AI agents should always read this document before performing any task.

---

# architecture/

## Purpose

Contains high-level technical and business architecture documentation.

Examples:

- System Overview
- Application Architecture
- Mobile Architecture
- Backend Architecture
- Deployment Flow
- Project Architecture

Purpose:

Help developers, QA engineers, and AI agents understand how the overall platform is designed.

---

# flows/

## Purpose

Contains detailed documentation for every business feature.

Each feature should have its own Markdown document.

Examples:

- Authentication
- Registration
- Login
- KYC
- Wallet
- Finix Payment
- Contest
- Draft
- Pick'em
- Props Booster
- Best Ball
- Rankings
- Notifications
- Admin Panel

Each document should follow the standard Flow Documentation Template.

---

# api/

## Purpose

Contains API documentation for every business module.

Documentation should include:

- Endpoint overview
- Request parameters
- Response schema
- Authentication requirements
- Validation rules
- Error responses
- Business logic

---

# automation/

## Purpose

Contains automation standards and implementation guidelines.

Examples:

- Appium Standards
- Playwright Standards
- Page Object Model
- Locator Strategy
- Coding Standards
- Automation Best Practices
- AI Prompt Library

---

# test-data/

## Purpose

Contains reusable QA resources.

Examples:

- Test Accounts
- Sample Test Data
- Mock Data
- Environment Configuration
- Test Cards
- Sports Data

Production credentials or sensitive information must never be stored in this directory.

---

# reports/

## Purpose

Contains report templates and QA documentation.

Examples:

- Regression Reports
- Smoke Test Reports
- Release Reports
- Defect Summary Reports
- Automation Execution Reports

---

# troubleshooting/

## Purpose

Contains common issues, known limitations, and troubleshooting guides.

Examples:

- Payment Issues
- Login Issues
- KYC Issues
- Draft Issues
- Notification Issues
- Known Limitations

---

# release-notes/

## Purpose

Maintains release documentation.

Examples:

- Feature Releases
- Bug Fix Releases
- Regression Summary
- Production Release Notes
- Rollback Notes

---

# Documentation Standards

Every document in this repository should:

- Have a clear purpose.
- Follow the standard documentation template.
- Be easy to understand.
- Be updated whenever the application changes.
- Include related documentation references where applicable.

---

# AI Repository Navigation

AI agents should navigate the repository in the following order:

1. README.md
2. AGENTS.md
3. architecture/
4. flows/
5. api/
6. automation/
7. test-data/
8. troubleshooting/
9. reports/
10. release-notes/

This ensures AI agents understand the project before generating code, automation, or documentation.

---

# Repository Maintenance

The repository should be updated whenever:

- A new feature is introduced.
- A business rule changes.
- A new API is added.
- A QA workflow changes.
- An automation standard is updated.
- A release introduces new functionality.

Maintaining accurate documentation ensures consistency across the Drafters engineering team.

# 5. Development Environment

## Overview

The Drafters platform follows a structured development and testing lifecycle to ensure feature quality, stability, and consistency across all supported platforms.

Development, testing, and deployment activities are performed in separate environments. AI agents and team members should always use the appropriate environment based on the task being performed.

---

# Supported Applications

The Drafters platform consists of the following applications:

- Web Application
- Android Application
- iOS Application
- Admin Portal
- Backend Services

Each application may have its own deployment cycle while following the same QA and release process.

---

# Development Lifecycle

The standard feature development workflow is:

```
Requirement
        │
        ▼
Business Analysis
        │
        ▼
Design
        │
        ▼
Development
        │
        ▼
Code Review
        │
        ▼
Deploy to Development Environment
        │
        ▼
Deploy to Staging Environment
        │
        ▼
QA Testing
        │
        ▼
Regression Testing
        │
        ▼
Business Approval
        │
        ▼
Production Deployment
```

---

# Development Environment

## Purpose

Used by developers during feature implementation and initial testing.

Typical Activities

- Feature Development
- Unit Testing
- Initial Bug Fix Verification
- Local Debugging

AI agents should not assume access to development environments unless explicitly provided.

---

# Staging Environment

## Purpose

Primary environment used by the QA team.

Typical Activities

- Functional Testing
- Regression Testing
- Smoke Testing
- API Validation
- Cross-platform Testing
- Release Verification

Unless instructed otherwise, AI-generated test cases and automation should target the Staging environment.

---

# Production Environment

## Purpose

Used by end users.

Typical Activities

- Production Verification
- Smoke Testing
- Release Monitoring
- Critical Issue Validation

Production should never be used for destructive testing or experimental validation.

---

# Platform Distribution

## Web

Accessed through the appropriate environment URL.

---

## Android

Distributed using QA-approved staging builds or APKs.

---

## iOS

Distributed through TestFlight or the approved internal distribution process.

---

## Admin Portal

Used by internal teams for configuration, reporting, and operational management.

---

# QA Responsibilities

During development and staging, QA engineers should verify:

- Feature functionality
- Business rules
- UI/UX consistency
- API behavior
- Cross-platform compatibility
- Performance observations
- Regression impact

---

# AI Agent Guidelines

Before generating automation or test cases, AI agents should:

- Identify the target environment.
- Confirm the supported platform.
- Verify feature availability.
- Follow documented business rules.
- Avoid assumptions about environment-specific configurations.

---

# Environment Best Practices

Always:

- Use approved QA environments.
- Verify application version before testing.
- Validate environment-specific configurations.
- Document environment details in reports.

Never:

- Use production for destructive testing.
- Assume feature parity without validation.
- Hardcode environment-specific values into automation.

---

# Related Documentation

- Environment URLs
- Deployment Workflow
- QA Guidelines
- Release Notes
- Test Data

# 6. Environment URLs

## Overview

The Drafters platform is deployed across multiple environments to support development, quality assurance, user acceptance testing, and production releases.

Each environment serves a specific purpose in the software development lifecycle. AI agents and team members should always verify the target environment before performing any testing, automation, or validation activities.

Actual URLs, credentials, and sensitive configuration values must never be stored in this repository.

---

# Environment Types

The Drafters platform currently supports the following environments:

- Development
- Staging
- Production

Additional environments may be introduced as the platform evolves.

---

# Development Environment

## Purpose

Used by developers during feature implementation and debugging.

### Components

| Component | Placeholder |
|------------|-------------|
| Web Application | `<DEV_WEB_URL>` |
| Backend API | `<DEV_API_URL>` |
| Admin Portal | `<DEV_ADMIN_URL>` |

### Typical Activities

- Feature Development
- Local Verification
- Unit Testing
- Initial Integration Testing

---

# Staging Environment

## Purpose

Primary QA environment used for feature validation before production release.

### Components

| Component | Placeholder |
|------------|-------------|
| Web Application | `<STAGING_WEB_URL>` |
| Backend API | `<STAGING_API_URL>` |
| Admin Portal | `<STAGING_ADMIN_URL>` |
| Android Build | `<STAGING_ANDROID_BUILD>` |
| iOS Build | `<TESTFLIGHT_STAGING_BUILD>` |

### Typical Activities

- Functional Testing
- Regression Testing
- Smoke Testing
- Cross-Platform Testing
- API Validation
- Automation Execution
- UAT Support

---

# Production Environment

## Purpose

Live environment used by end users.

### Components

| Component | Placeholder |
|------------|-------------|
| Web Application | `<PRODUCTION_WEB_URL>` |
| Backend API | `<PRODUCTION_API_URL>` |
| Admin Portal | `<PRODUCTION_ADMIN_URL>` |

### Typical Activities

- Production Verification
- Smoke Testing
- Production Monitoring
- Critical Issue Validation

Production should never be used for destructive testing or experimental validation.

---

# Environment Configuration

Each environment may have different:

- Feature Flags
- Payment Configurations
- KYC Configurations
- Responsible Gaming Rules
- Notification Settings
- Third-Party Integrations
- Test Data

AI agents should never assume configuration parity between environments.

---

# Environment Validation Checklist

Before starting any testing, verify:

- Correct environment
- Correct application version
- Correct build number
- Required feature flags enabled
- Required test accounts available
- Required test data available

---

# Security Guidelines

This repository must never contain:

- Production URLs
- User credentials
- API Keys
- Access Tokens
- Secret Keys
- Database Credentials

Environment-specific values should be managed using secure configuration management systems.

---

# AI Agent Instructions

Before generating automation or test cases, AI agents should:

1. Confirm the target environment.
2. Verify platform availability.
3. Validate environment-specific configurations.
4. Use approved QA environments.
5. Never execute destructive operations against Production.

---

# Related Documentation

- Development Environment
- Deployment Workflow
- Test Data
- Safety Rules

# 7. Authentication & User Roles

## Overview

Authentication is the process of verifying a user's identity before granting access to protected resources within the Drafters platform.

The Drafters platform uses role-based access control (RBAC) to ensure users can only access features and functionality permitted for their assigned role.

AI agents should understand the authentication workflow, user roles, and authorization rules before generating automation, test cases, or reviewing feature implementations.

---

# Authentication Methods

The Drafters platform supports secure authentication across all supported platforms.

Supported Platforms

- Web
- Android
- iOS
- Admin Portal

Authentication is required before users can access protected features such as:

- Wallet
- Payments
- Contest Participation
- Draft
- Pick'em
- User Profile
- Admin Portal

---

# User Roles

The platform supports multiple user roles.

## 1. End User

Purpose

Fantasy sports users who participate in contests.

Permissions

- Register
- Login
- Manage Profile
- Complete KYC
- Deposit Funds
- Withdraw Funds
- Join Contests
- Draft Players
- Create Pick'em Entries
- View Rankings
- View Notifications

Supported Platforms

- Web
- Android
- iOS

---

## 2. Administrator

Purpose

Manage platform operations and configurations.

Permissions

- Manage Users
- Manage Contests
- Configure Promotions
- Configure Responsible Gaming
- Manage Payments
- Configure Feature Flags
- View Reports
- Monitor Platform Activity

Supported Platforms

- Admin Portal

---

## 3. QA Engineer

Purpose

Validate application functionality before release.

Permissions

- Execute Functional Testing
- Execute Regression Testing
- Validate APIs
- Execute Automation
- Verify Release Builds
- Perform Smoke Testing

QA Engineers should always use approved QA environments and test accounts.

---

## 4. Developer

Purpose

Implement and maintain application features.

Responsibilities

- Develop Features
- Fix Defects
- Review Code
- Support QA
- Maintain APIs

---

# Authentication Flow

A standard authentication flow consists of:

1. User enters credentials.
2. Credentials are validated.
3. User is authenticated.
4. Session is established.
5. User gains access based on assigned role.

If authentication fails:

- Appropriate error messages should be displayed.
- Access to protected resources should be denied.

---

# Authorization

Authorization determines which resources a user can access after successful authentication.

AI agents should verify:

- Role-based access control.
- Restricted page access.
- Unauthorized access handling.
- Session validation.
- Permission enforcement.

---

# Session Management

Verify the following:

- Session created after successful login.
- Session expires according to application configuration.
- Logout invalidates the active session.
- Expired sessions redirect users to the login page.

---

# QA Validation Checklist

Verify:

- Valid Login
- Invalid Login
- Required Field Validation
- Password Validation
- Session Expiration
- Logout Functionality
- Unauthorized Access
- Role-Based Permissions
- Authentication Error Messages

---

# Security Guidelines

Authentication documentation must never contain:

- Production Credentials
- Test Passwords
- API Keys
- Authentication Tokens
- Secret Keys

Sensitive credentials should be managed using approved secure storage solutions.

---

# AI Agent Instructions

Before generating authentication automation or test cases, AI agents should:

- Identify the user role.
- Verify authentication requirements.
- Validate role-based permissions.
- Consider platform-specific authentication behavior.
- Use approved QA accounts.
- Never hardcode credentials in generated code or documentation.

---

# Related Documentation

- flows/authentication.md
- flows/login.md
- flows/registration.md
- flows/forgot-password.md
- flows/profile.md
- api/authentication.md
- test-data/qa-accounts.md

# 8. Business Domains

## Overview

The Drafters platform consists of multiple business domains that work together to provide a complete fantasy sports experience across Web, Android, iOS, and the Admin Portal.

Each business domain has a specific purpose, business rules, APIs, user journeys, and automation requirements.

Detailed documentation for each domain is maintained in the `flows/` directory.

AI agents should always review the relevant flow documentation before generating automation, reviewing code, or analyzing defects.

---

# Business Domain Overview

| Domain | Purpose | Documentation |
|---------|---------|---------------|
| Authentication | Secure user access and session management | `flows/authentication.md` |
| Registration | User onboarding and account creation | `flows/registration.md` |
| Login | User authentication | `flows/login.md` |
| Forgot Password | Password recovery process | `flows/forgot-password.md` |
| User Profile | Profile management and account settings | `flows/profile.md` |
| KYC | Identity verification and compliance | `flows/kyc.md` |
| Wallet | Manage user balance and transactions | `flows/wallet.md` |
| Finix Payment | Card payment processing | `flows/finix-payment.md` |
| PayPal | Alternative payment method | `flows/paypal.md` |
| Contest Lobby | Browse available contests | `flows/lobby.md` |
| Contest | Contest creation and participation | `flows/contest.md` |
| Draft | Player drafting workflow | `flows/draft.md` |
| Slow Draft | Long-duration drafting | `flows/slow-draft.md` |
| Fast Draft | Real-time drafting | `flows/fast-draft.md` |
| Best Ball | Best Ball fantasy contests | `flows/best-ball.md` |
| Best Ball Survival | Survival tournament mode | `flows/best-ball-survival.md` |
| Pick'em | Player prediction contests | `flows/pickem.md` |
| Props | Player proposition picks | `flows/props.md` |
| Props Booster | Promotional boosters | `flows/props-booster.md` |
| Rankings | Player and contest rankings | `flows/rankings.md` |
| Leaderboard | Leaderboard and standings | `flows/leaderboard.md` |
| Notifications | Push, email, and in-app notifications | `flows/notifications.md` |
| Rewards | User rewards and promotions | `flows/rewards.md` |
| Responsible Gaming | Deposit limits and compliance | `flows/responsible-gaming.md` |
| Admin Portal | Platform administration | `flows/admin-panel.md` |

---

# Business Domain Dependencies

The following diagram shows how major modules interact.

```

Authentication
│
├── Registration
├── Login
├── Profile
├── KYC
│
▼

Wallet
│
├── Finix Payment
├── PayPal
├── Rewards
└── Responsible Gaming
│
▼

Contest Lobby
│
▼

Contest
│
▼

Draft
│
├── Slow Draft
├── Fast Draft
├── Best Ball
├── Best Ball Survival
├── Pick'em
├── Props
└── Props Booster
│
▼

Rankings
│
▼

Leaderboard
│
▼

Notifications

```

---

# Platform Coverage

| Business Domain | Web | Android | iOS | Admin |
|-----------------|:---:|:-------:|:---:|:-----:|
| Authentication | ✅ | ✅ | ✅ | ✅ |
| Registration | ✅ | ✅ | ✅ | ❌ |
| Profile | ✅ | ✅ | ✅ | ❌ |
| KYC | ✅ | ✅ | ✅ | ✅ |
| Wallet | ✅ | ✅ | ✅ | ❌ |
| Payments | ✅ | ✅ | ✅ | ✅ |
| Contest | ✅ | ✅ | ✅ | ✅ |
| Draft | ✅ | ✅ | ✅ | ❌ |
| Pick'em | ✅ | ✅ | ✅ | ❌ |
| Props Booster | ✅ | ✅ | ✅ | ✅ |
| Rankings | ✅ | ✅ | ✅ | ❌ |
| Notifications | ✅ | ✅ | ✅ | ✅ |
| Responsible Gaming | ✅ | ✅ | ✅ | ✅ |

---

# AI Agent Responsibilities

Before working on any feature, AI agents should:

1. Identify the affected business domain.
2. Read the corresponding document in the `flows/` directory.
3. Review related APIs (if applicable).
4. Understand business rules and validations.
5. Consider platform-specific behavior.
6. Follow documented automation standards.
7. Generate outputs consistent with project guidelines.

---

# Documentation Standards

Every business domain document must include the following sections:

1. Overview
2. Business Purpose
3. User Flow
4. UI Screens
5. Backend APIs
6. Business Rules
7. Validation Rules
8. Positive Scenarios
9. Negative Scenarios
10. Edge Cases
11. Error Messages
12. Platform Differences
13. Admin Configuration
14. Test Data
15. Automation Strategy
16. Related Modules
17. Known Issues
18. Future Enhancements

All business domain documents should follow this standard template to ensure consistency across the repository.

---

# Related Documentation

- `architecture/system-overview.md`
- `flows/`
- `api/`
- `automation/`
- `test-data/`

# 9. Business Rules

## Overview

Business rules define the expected behavior of the Drafters platform and ensure consistency across Web, Android, iOS, and the Admin Portal.

These rules serve as the foundation for feature implementation, quality assurance, automation, and AI-assisted analysis.

This section provides a high-level overview of the core business rules. Detailed business rules, validations, workflows, and feature-specific behavior are documented in the corresponding files under the `flows/` directory.

---

## General Business Rules

The following rules apply across the Drafters platform unless otherwise specified:

- Users must be authenticated before accessing protected features.
- Business logic should remain consistent across Web, Android, iOS, and Admin Portal.
- All critical business actions should generate the expected system response.
- Failed operations must not leave the system in an inconsistent state.
- User-facing validation messages should be clear and meaningful.
- Role-based access control (RBAC) must be enforced.
- All financial transactions must be recorded appropriately.
- Platform-specific behavior should follow documented business requirements.

---

## Authentication & User Management

### Business Rules

- Users must complete registration before accessing protected features.
- Login is required to access user-specific modules.
- User profile information should remain synchronized across supported platforms.
- Unauthorized users must not access restricted resources.
- Sessions must be securely managed and expire according to platform configuration.

**Reference Documentation**

- flows/authentication.md
- flows/registration.md
- flows/login.md
- flows/profile.md

---

## Identity Verification (KYC)

### Business Rules

- KYC verification is required where applicable by business or regulatory requirements.
- Financial features may be restricted until verification is completed.
- KYC status should remain consistent across all supported platforms.
- Verification failures should display appropriate guidance to users.

**Reference Documentation**

- flows/kyc.md

---

## Wallet & Payments

### Business Rules

- Wallet balance must never become negative.
- Successful deposits must correctly update wallet balance.
- Failed payment attempts must not credit the wallet.
- Refunds must follow documented business rules.
- Every financial transaction should appear in transaction history.
- Payment providers should follow their configured integration workflows.

**Reference Documentation**

- flows/wallet.md
- flows/finix-payment.md
- flows/paypal.md

---

## Contest & Lobby

### Business Rules

- Only eligible users may join contests.
- Contest availability depends on business configuration.
- Entry fees should only be deducted after a successful contest entry.
- Contest lifecycle must follow configured business rules.
- Contest information should remain synchronized across supported platforms.

**Reference Documentation**

- flows/lobby.md
- flows/contest.md

---

## Draft

### Business Rules

- Drafts must begin according to contest configuration.
- Draft order must follow configured draft settings.
- A player cannot be drafted more than once in the same draft.
- Auto Pick must execute after the configured pick timer expires.
- Draft status should update correctly throughout the draft lifecycle.

**Reference Documentation**

- flows/draft.md
- flows/slow-draft.md
- flows/fast-draft.md
- flows/best-ball.md
- flows/best-ball-survival.md

---

## Pick'em & Props

### Business Rules

- Users may submit entries only when all validation rules are satisfied.
- Entry validation should follow configured business rules.
- Props Boosters should apply only when eligibility requirements are met.
- Contest settlement should follow official scoring rules.
- Push, Void, Refund, Safety, and Revive scenarios must follow documented feature rules.

**Reference Documentation**

- flows/pickem.md
- flows/props.md
- flows/props-booster.md

---

## Rankings & Leaderboards

### Business Rules

- Rankings should reflect the latest available contest results.
- Leaderboards should update after scoring is completed.
- Ranking calculations should remain consistent across supported platforms.

**Reference Documentation**

- flows/rankings.md
- flows/leaderboard.md

---

## Responsible Gaming

### Business Rules

- Responsible Gaming controls must be enforced where configured.
- Deposit limits should follow configured daily, weekly, monthly, and yearly limits.
- Restricted users must not bypass Responsible Gaming restrictions.

**Reference Documentation**

- flows/responsible-gaming.md

---

## Notifications

### Business Rules

- Notifications should be generated based on configured events.
- Duplicate notifications should not be created.
- Notification delivery should respect user preferences where supported.

**Reference Documentation**

- flows/notifications.md

---

## Admin Portal

### Business Rules

- Administrative actions must be restricted to authorized users.
- Configuration changes should propagate correctly to supported applications.
- Administrative changes must follow documented approval and deployment processes.

**Reference Documentation**

- flows/admin-panel.md

---

## AI Agent Instructions

Before generating automation, test cases, code reviews, or business analysis, AI agents should:

- Identify the relevant business domain.
- Review the corresponding documentation under the `flows/` directory.
- Follow documented business rules and validations.
- Consider platform-specific behavior.
- Avoid assumptions that are not documented.
- Report business rule violations separately from UI or implementation issues.

---

## Detailed Business Rules

This section provides only a high-level overview of the Drafters business rules.

Complete feature-specific documentation, including workflows, validations, edge cases, error handling, and business logic, is maintained in the corresponding files under the `flows/` directory.

AI agents and team members should always refer to the relevant feature documentation before generating automation, test cases, or implementation recommendations.

---

## Related Documentation

- flows/
- api/
- Frontend QA Guidelines
- API QA Guidelines
- Database Validation
- Architecture Documentation

# 10. Frontend QA Guidelines

## Overview

This section defines the standard Quality Assurance (QA) practices for validating the Drafters platform across all supported client applications.

The objective is to ensure consistent functionality, business rule compliance, usability, and user experience across Web, Android, iOS, and the Admin Portal.

All manual testing, automation testing, regression testing, and AI-generated test cases should follow these guidelines.

---

# Supported Platforms

Frontend validation should be performed for the following applications:

- Web Application
- Android Application
- iOS Application
- Admin Portal

Unless a feature is platform-specific, behavior should remain consistent across all supported platforms.

---

# QA Testing Objectives

Every feature should be validated for:

- Functional correctness
- Business rule compliance
- UI consistency
- Navigation flow
- Data accuracy
- Cross-platform compatibility
- Performance observations
- Error handling
- Accessibility (where applicable)
- Overall user experience

---

# Standard User Journey Validation

Each feature should be tested using the complete user journey.

Typical workflow:

```
Launch Application
        │
        ▼
Authentication
        │
        ▼
Feature Access
        │
        ▼
User Interaction
        │
        ▼
Backend Processing
        │
        ▼
UI Validation
        │
        ▼
Success / Failure Validation
        │
        ▼
Data Verification
```

Every user journey should complete successfully without unexpected interruptions.

---

# Core QA Validation Checklist

The following validations should be performed for every feature whenever applicable.

## Functional Validation

Verify:

- Feature works as expected.
- Business rules are correctly implemented.
- User actions produce expected results.
- Data is displayed correctly.
- State changes occur correctly.
- Feature behaves consistently.

---

## UI Validation

Verify:

- Layout is correct.
- Fonts are consistent.
- Colors follow design guidelines.
- Icons display correctly.
- Images load correctly.
- Buttons are properly aligned.
- Labels and text are correct.
- No overlapping UI elements.
- No truncation issues.

---

## Navigation Validation

Verify:

- Navigation follows expected workflow.
- Back navigation behaves correctly.
- Deep links open the correct screens.
- External links function correctly.
- Navigation state is maintained.

---

## Input Validation

Verify:

- Required fields.
- Invalid input.
- Boundary values.
- Character limits.
- Special characters.
- Empty fields.
- Input formatting.
- Keyboard behavior on mobile.

---

## API Validation

Verify:

- Correct API requests are triggered.
- Successful responses update the UI.
- Failed responses display appropriate messages.
- No unexpected API failures.
- Loading states behave correctly.

---

## Error Handling

Verify:

- Error messages are user-friendly.
- Validation messages are meaningful.
- Retry functionality works correctly.
- Unexpected failures are handled gracefully.
- Application does not crash.

---

## Loading State Validation

Verify:

- Loading indicators appear correctly.
- Loaders disappear after completion.
- Duplicate requests are prevented.
- Users receive visual feedback while processing.

---

## Cross-Platform Validation

Verify consistency between:

- Web
- Android
- iOS

Check for:

- Business logic
- UI behavior
- Validation messages
- Navigation
- Calculations
- Feature availability

Document any platform-specific differences.

---

# Regression Testing

Regression testing should verify that new changes do not impact existing functionality.

Areas to validate include:

- Authentication
- Wallet
- Payments
- Contest
- Draft
- Pick'em
- Props
- Rankings
- Notifications
- Profile
- Responsible Gaming

Regression scope should be determined based on the feature being released.

---

# AI Agent Responsibilities

Before generating frontend automation or manual test cases, AI agents should:

- Review the relevant feature documentation.
- Follow documented business rules.
- Consider platform-specific behavior.
- Generate reusable and maintainable test cases.
- Include positive, negative, and edge case scenarios.
- Avoid undocumented assumptions.

---

# Expected QA Deliverables

Frontend validation should result in:

- Test Cases
- Test Execution Report
- Defect Report
- Regression Report
- Screenshots (when applicable)
- Screen Recordings (for reproducible issues)
- Platform Comparison Report
- Release Validation Summary

---

# General QA Best Practices

Always verify:

- No console errors.
- No failed API requests (unless expected).
- No broken images or icons.
- No JavaScript exceptions.
- Correct navigation.
- Correct data rendering.
- Responsive layouts where applicable.
- Proper loading indicators.
- Correct success and error messages.
- Application stability.

---

# Related Documentation

- flows/
- api/
- automation/
- reports/
- release-notes/
