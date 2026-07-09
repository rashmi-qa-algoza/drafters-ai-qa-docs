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

# 11. API QA Guidelines

## Overview

This section defines the standard API Quality Assurance (QA) guidelines for the Drafters platform.

All backend APIs should be validated to ensure they meet functional requirements, business rules, security standards, and performance expectations.

These guidelines apply to all APIs used by the Web Application, Android Application, iOS Application, and Admin Portal.

---

# API Testing Objectives

The primary objectives of API testing are to verify:

- Functional correctness
- Business rule compliance
- Data integrity
- Security
- Performance
- Reliability
- Error handling
- Backward compatibility

---

# Standard API Validation Checklist

Every API should be validated for the following:

## Request Validation

Verify:

- Correct HTTP Method (GET, POST, PUT, PATCH, DELETE)
- Required headers
- Authentication token
- Request body
- Query parameters
- Path parameters
- Request schema validation

---

## Response Validation

Verify:

- Correct HTTP Status Code
- JSON response format
- Response schema
- Required response fields
- Correct data types
- Expected business data
- Pagination (where applicable)

---

## Authentication & Authorization

Verify:

- Authorized users can access the API.
- Unauthorized requests return appropriate error codes.
- Invalid or expired tokens are rejected.
- Role-based permissions are enforced.
- Protected APIs require authentication.

---

## Business Logic Validation

Verify:

- Business rules are correctly implemented.
- Invalid operations are rejected.
- Duplicate operations are handled correctly.
- State changes are accurate.
- Data consistency is maintained.

---

## Input Validation

Verify:

- Required fields
- Empty values
- Invalid values
- Maximum length
- Minimum length
- Invalid data types
- Boundary values
- Special characters
- SQL Injection protection
- XSS protection (where applicable)

---

## Error Handling

Verify:

- Meaningful error messages
- Appropriate HTTP status codes
- No internal implementation details exposed
- No stack traces returned
- Consistent error response format

---

## Data Validation

Verify:

- Data is correctly stored.
- Data is correctly updated.
- Data is correctly deleted.
- Data is returned accurately.
- Duplicate records are prevented where applicable.

---

## API Performance

Verify:

- Response time meets project expectations.
- Large datasets are handled efficiently.
- Pagination performs correctly.
- No unnecessary delays.

---

## Security Validation

Verify:

- Authentication enforcement
- Authorization checks
- Sensitive data masking
- Secure transport (HTTPS)
- Input sanitization
- Rate limiting (where applicable)

---

# Common HTTP Status Codes

| Status Code | Description |
|-------------|-------------|
| 200 | Success |
| 201 | Resource Created |
| 204 | No Content |
| 400 | Bad Request |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |
| 409 | Conflict |
| 422 | Validation Error |
| 429 | Too Many Requests |
| 500 | Internal Server Error |

---

# API Regression Testing

Regression testing should verify that API changes do not impact:

- Authentication
- User Management
- Wallet
- Payments
- Contest
- Draft
- Pick'em
- Notifications
- Rankings
- Responsible Gaming
- Admin APIs

---

# AI Agent Responsibilities

Before generating API test cases or automation, AI agents should:

- Review the relevant API documentation.
- Understand the associated business rules.
- Validate both positive and negative scenarios.
- Consider edge cases and boundary conditions.
- Verify API security requirements.
- Generate reusable API test cases.
- Avoid assumptions not supported by documentation.

---

# API Testing Tools

Recommended tools include:

- Postman
- Swagger / OpenAPI
- cURL
- Playwright API Testing
- Cypress API Testing

The selected tool should follow the project's testing standards.

---

# Related Documentation

- api/
- flows/
- automation/
- Business Rules
- Database Validation

# 12. Database Validation

## Overview

Database validation ensures that business operations correctly create, update, retrieve, and maintain data consistency throughout the Drafters platform.

Although QA activities primarily focus on frontend and API validation, database verification should be performed whenever backend data integrity is critical to business functionality.

AI agents should understand the expected database behavior but should never directly modify production databases.

---

# Objectives

Database validation aims to verify:

- Data integrity
- Data consistency
- Business rule enforcement
- Transaction accuracy
- Relationship consistency
- Audit information
- Data synchronization across services

---

# General Validation Principles

After every successful business operation, AI agents and QA engineers should verify that:

- Expected records are created.
- Existing records are updated correctly.
- No duplicate records are created.
- Invalid operations do not modify data.
- Relationships between entities remain consistent.
- Transaction history is accurate.
- Audit information is updated where applicable.

---

# Authentication

Verify:

- User session is created.
- Login timestamp is updated.
- Failed login attempts do not modify user profile information.
- Logout invalidates the active session.

Reference:

- flows/authentication.md
- api/authentication.md

---

# Registration

Verify:

- User account is created.
- Duplicate accounts are prevented.
- Default profile information is initialized.
- Registration timestamp is recorded.
- Account status is correctly assigned.

Reference:

- flows/registration.md

---

# User Profile

Verify:

- Profile updates are saved successfully.
- Only modified fields are updated.
- Invalid updates do not corrupt user data.
- Audit fields are maintained.

Reference:

- flows/profile.md

---

# KYC

Verify:

- Verification status is updated.
- Submitted documents are associated with the correct user.
- Verification history is maintained.
- Failed verification does not incorrectly update account status.

Reference:

- flows/kyc.md

---

# Wallet

Verify:

- Wallet balance is updated correctly.
- Transaction records are created.
- Transaction amount is accurate.
- Transaction status matches business outcome.
- Failed transactions do not affect wallet balance.

Reference:

- flows/wallet.md

---

# Payments

Verify:

- Payment record is created.
- Payment status is updated.
- Duplicate transactions are prevented.
- Refund records follow business rules.
- Settlement information is maintained where applicable.

Reference:

- flows/finix-payment.md
- flows/paypal.md

---

# Contest

Verify:

- Contest entry is created.
- Entry fee transaction is recorded.
- Contest participant count is updated.
- Contest status reflects current lifecycle.

Reference:

- flows/contest.md

---

# Draft

Verify:

- Draft entry is created.
- Draft status is updated correctly.
- Player selections are stored accurately.
- Duplicate player selections are prevented.
- Pick history is maintained.

Reference:

- flows/draft.md

---

# Pick'em & Props

Verify:

- Entry is created successfully.
- Pick selections are stored.
- Contest status is updated correctly.
- Settlement updates the entry accurately.
- Booster eligibility follows business rules.

Reference:

- flows/pickem.md
- flows/props.md
- flows/props-booster.md

---

# Rankings

Verify:

- Rankings are updated after scoring.
- Leaderboards reflect latest results.
- Score calculations remain consistent.

Reference:

- flows/rankings.md
- flows/leaderboard.md

---

# Notifications

Verify:

- Notification records are created.
- Delivery status is updated.
- Duplicate notifications are prevented.

Reference:

- flows/notifications.md

---

# Responsible Gaming

Verify:

- Deposit limits are stored correctly.
- Restriction status is updated.
- User settings are applied consistently.

Reference:

- flows/responsible-gaming.md

---

# Database Validation Checklist

When database access is available, verify:

- Record Creation
- Record Update
- Record Deletion (where applicable)
- Data Integrity
- Foreign Key Relationships
- Duplicate Prevention
- Audit Information
- Transaction Consistency

If direct database access is unavailable, validate expected behavior through APIs or application UI.

---

# AI Agent Responsibilities

Before performing database validation, AI agents should:

- Understand the related business workflow.
- Review the corresponding flow documentation.
- Validate expected data changes.
- Verify data consistency after business operations.
- Report any unexpected data modifications.
- Never recommend or perform direct production database changes.

---

# Security Guidelines

AI agents must never:

- Modify production database records.
- Delete production data.
- Execute destructive database queries.
- Store database credentials in documentation.
- Expose sensitive user information.

---

# Related Documentation

- flows/
- api/
- Business Rules
- API QA Guidelines
- Safety Rules

# 13. Logging Requirements

## Overview

Logs play a critical role in identifying, diagnosing, and resolving issues within the Drafters platform.

During manual testing, automation execution, API validation, and production verification, AI agents and QA engineers should review relevant logs to identify unexpected behavior, application failures, performance issues, and integration problems.

Whenever possible, reported defects should include supporting log evidence.

---

# Logging Objectives

Logging should help identify:

- Application errors
- API failures
- Authentication issues
- Payment failures
- Third-party integration issues
- Performance bottlenecks
- Unexpected exceptions
- Data inconsistencies

---

# Browser Console Logs (Web)

For Web Application testing, verify:

- No JavaScript exceptions
- No uncaught runtime errors
- No failed resource loading
- No unexpected console errors
- No deprecated API warnings affecting functionality

Report:

- JavaScript Errors
- Console Exceptions
- Failed Resource Requests
- Critical Warnings

Ignore:

- Browser extension warnings
- Documented third-party library warnings
- Informational console messages

---

# Network Logs

Review browser network activity and verify:

- API request is triggered
- Correct request payload
- Correct response payload
- HTTP status code
- Response time
- Authentication headers
- No failed API requests
- No duplicate API requests

Report:

- 4xx Errors
- 5xx Errors
- Timeout Errors
- Invalid Response Structure

---

# Android Logs

Review Android device logs (Logcat) and verify:

- No application crashes
- No ANR (Application Not Responding)
- No fatal exceptions
- No repeated runtime errors
- No unexpected SDK failures

Report:

- Fatal Exceptions
- Crash Logs
- Memory Issues
- Runtime Exceptions

Ignore:

- Informational logs
- Debug logs
- Documented SDK warnings

---

# iOS Logs

Review iOS device or TestFlight logs and verify:

- No application crashes
- No fatal runtime exceptions
- No unexpected framework errors
- Stable application behavior

Report:

- Crash Logs
- Fatal Exceptions
- Runtime Errors

Ignore:

- Apple framework informational logs
- Known simulator warnings (when applicable)

---

# Backend Logs

When backend access is available, verify:

- API execution
- Business validation failures
- Authentication failures
- Payment processing
- Database exceptions
- Integration failures
- Internal server errors

Report:

- Unhandled Exceptions
- Database Errors
- API Processing Errors
- Integration Failures

---

# Third-Party Integration Logs

Review logs for integrated services where available.

Examples include:

- Payment Gateway
- KYC Provider
- Push Notification Services
- Email Services

Verify:

- Request Success
- Response Status
- Timeout Handling
- Authentication
- Retry Mechanisms

---

# Performance Logs

Verify:

- Slow API responses
- High response times
- Memory usage (where available)
- CPU utilization (where available)
- Network latency

Report noticeable performance degradation.

---

# Defect Reporting Requirements

When reporting issues, include:

- Platform
- Environment
- Build Version
- Timestamp
- Relevant Logs
- Console Output
- API Response
- Error Message
- Screenshot
- Screen Recording (if available)

Providing supporting evidence improves issue investigation and resolution.

---

# AI Agent Responsibilities

When analyzing failures, AI agents should:

- Review relevant logs before drawing conclusions.
- Correlate log entries with user actions.
- Identify the probable root cause.
- Distinguish between application issues and third-party failures.
- Highlight critical errors separately from warnings.
- Include relevant log excerpts in reports when appropriate.

AI agents should never ignore critical exceptions or server-side errors.

---

# Logging Best Practices

Always:

- Capture logs immediately after reproducing an issue.
- Include timestamps in reports.
- Verify logs from the correct environment.
- Attach supporting evidence with reported defects.
- Protect sensitive information before sharing logs.

Never:

- Share authentication tokens.
- Share production credentials.
- Include personally identifiable information (PII) in reports.
- Modify or delete production logs.

---

# Related Documentation

- Frontend QA Guidelines
- API QA Guidelines
- Database Validation
- Troubleshooting
- Reporting Format

# 14. Performance Expectations

## Overview

The Drafters platform should provide a fast, stable, and responsive experience across Web, Android, iOS, and the Admin Portal.

Performance validation ensures that application features, APIs, and user interactions meet acceptable response times while maintaining reliability under normal operating conditions.

AI agents and QA engineers should monitor performance throughout functional testing, regression testing, and production verification.

---

# Performance Objectives

Performance validation should ensure:

- Fast application response times
- Smooth user experience
- Stable application behavior
- Efficient resource utilization
- Reliable API performance
- Consistent cross-platform performance

---

# Application Performance

Verify:

- Application launches successfully.
- Screens load within acceptable time.
- Navigation between screens is smooth.
- UI interactions respond without noticeable delay.
- No unexpected freezes or crashes occur.

Expected Results

- Responsive UI
- Smooth transitions
- Stable application behavior
- Consistent performance across supported platforms

---

# Web Performance

Verify:

- Homepage loads successfully.
- Contest Lobby loads efficiently.
- Dashboard pages render correctly.
- Images and static assets load completely.
- Browser remains responsive during navigation.

Monitor:

- Initial page load
- Navigation speed
- Resource loading
- Browser responsiveness

---

# Mobile Performance

Verify on both Android and iOS:

- Application startup time
- Screen transition performance
- Scroll performance
- Animation smoothness
- Memory stability
- Battery usage (where applicable)

Ensure:

- No Application Not Responding (ANR)
- No unexpected crashes
- No excessive loading delays

---

# API Performance

Verify:

- APIs respond within acceptable response times.
- Requests do not timeout unexpectedly.
- Retry mechanisms work correctly.
- Multiple requests are handled efficiently.

Monitor:

- Response Time
- Latency
- Error Rate
- Throughput

---

# Authentication Performance

Verify:

- Login completes successfully.
- Registration completes within acceptable time.
- Session validation is responsive.
- Logout completes without delay.

---

# Wallet & Payment Performance

Verify:

- Wallet information loads quickly.
- Payment processing completes without unnecessary delay.
- Transaction history loads efficiently.
- Balance updates promptly after successful transactions.

Monitor:

- Payment processing time
- Wallet synchronization
- Transaction updates

---

# Contest Performance

Verify:

- Contest Lobby loads efficiently.
- Contest details open quickly.
- Contest joining completes successfully.
- Contest status updates correctly.

---

# Draft Performance

Verify:

- Draft room loads before draft begins.
- Player search responds efficiently.
- Player selection updates immediately.
- Draft timers remain synchronized.
- Auto Pick executes according to configuration.

---

# Pick'em & Props Performance

Verify:

- Pick selection is responsive.
- Entry submission completes successfully.
- Contest settlement updates correctly.
- Props Booster calculations do not impact responsiveness.

---

# Notification Performance

Verify:

- Notifications are delivered promptly.
- Notification lists load correctly.
- Notification status updates without delay.

---

# Performance Monitoring

Where applicable, monitor:

- Page Load Time
- API Response Time
- Memory Usage
- CPU Utilization
- Network Latency
- Crash Rate

---

# Performance Regression

AI agents and QA engineers should identify:

- Slower response times
- Increased loading times
- Memory leaks
- Performance degradation after releases
- UI responsiveness issues
- Excessive API latency

Performance regressions should be reported with supporting evidence.

---

# AI Agent Responsibilities

Before reporting performance issues, AI agents should:

- Compare current performance with previous releases when possible.
- Differentiate between application issues and network-related delays.
- Include performance observations in QA reports.
- Provide relevant screenshots, logs, or timing information.

AI agents should report significant performance degradation that impacts user experience.

---

# Performance Best Practices

Always:

- Verify performance on supported platforms.
- Test under normal network conditions.
- Validate loading indicators.
- Monitor API response times.
- Observe application stability during extended usage.

Never:

- Assume performance issues without supporting evidence.
- Ignore repeated slow responses.
- Overlook platform-specific performance differences.

---

# Related Documentation

- Frontend QA Guidelines
- API QA Guidelines
- Logging Requirements
- Deployment Workflow
- Reporting Format

# 15. Coding Standards

## Overview

This section defines the coding and documentation standards that should be followed across the Drafters platform.

The objective is to ensure that all code, automation scripts, documentation, and AI-generated outputs are consistent, maintainable, reusable, and easy to understand.

AI agents should follow these standards when generating code, automation, documentation, or implementation recommendations.

---

# General Principles

All code and documentation should be:

- Simple and easy to understand.
- Modular and reusable.
- Consistent across the project.
- Well-structured and maintainable.
- Easy to review and extend.

Avoid:

- Duplicate code
- Hardcoded values
- Unnecessary complexity
- Unused code
- Poor naming conventions

---

# Naming Conventions

Use meaningful and descriptive names for:

- Classes
- Methods
- Variables
- Constants
- Test Cases
- Page Objects
- API Clients
- Documentation Files

Examples:

- LoginPage
- WalletPage
- DraftPage
- PaymentService
- verifySuccessfulLogin()
- submitPickemEntry()

Avoid generic names such as:

- test1
- temp
- data
- value
- obj

---

# Code Organization

Code should be organized into logical modules.

Recommended structure:

- Business Logic
- Page Objects
- API Clients
- Utilities
- Test Data
- Test Cases
- Configuration

Each component should have a single responsibility.

---

# Reusability

Reusable components should be created for:

- Common UI interactions
- API requests
- Authentication
- Test data generation
- Assertions
- Utility methods
- Reporting

Avoid duplicating the same logic across multiple files.

---

# Configuration Management

Configuration should be separated from implementation.

Examples include:

- Environment configuration
- Base URLs
- Timeouts
- Feature flags
- Test accounts

Sensitive information must never be hardcoded.

---

# Test Design Standards

Automated tests should:

- Validate one business scenario per test.
- Be independent and repeatable.
- Use reusable helper methods.
- Include meaningful assertions.
- Avoid unnecessary dependencies.

Test execution should produce consistent results.

---

# Assertions

Assertions should:

- Clearly validate expected behavior.
- Produce meaningful failure messages.
- Verify business outcomes instead of implementation details.
- Be easy to understand.

---

# Synchronization

Automation should prefer:

- Explicit waits
- Element state validation
- API synchronization
- Event-based synchronization

Avoid:

- Fixed delays
- Excessive sleep statements
- Unnecessary retries

---

# Logging

Automation should log:

- Test execution steps
- User actions
- API requests
- Validation results
- Failure details

Logs should help identify failures without exposing sensitive information.

---

# Error Handling

Code should:

- Handle expected exceptions gracefully.
- Fail with meaningful error messages.
- Capture sufficient debugging information.
- Avoid suppressing unexpected exceptions.

---

# Documentation Standards

All documentation should:

- Follow the approved repository template.
- Be written in clear and concise language.
- Use consistent terminology.
- Be updated whenever functionality changes.
- Include references to related documentation.

---

# AI Agent Responsibilities

When generating code or documentation, AI agents should:

- Follow project naming conventions.
- Generate reusable and maintainable code.
- Follow documented business rules.
- Avoid unnecessary complexity.
- Reuse existing components whenever possible.
- Clearly explain assumptions when required.

AI agents should never generate code that violates documented project standards.

---

# Best Practices

Always:

- Write readable code.
- Use meaningful names.
- Keep methods small and focused.
- Reuse existing utilities.
- Follow project conventions.
- Update documentation with code changes.

Never:

- Hardcode credentials.
- Duplicate business logic.
- Ignore coding standards.
- Generate undocumented functionality.

---

# Related Documentation

- AGENTS.md
- automation/
- flows/
- api/
- templates/

# 16. Deployment Workflow

## Overview

The Drafters platform follows a structured Software Development Life Cycle (SDLC) to ensure every feature is reviewed, tested, and validated before being released to production.

This workflow helps maintain application quality, minimize production issues, and ensure consistent releases across Web, Android, iOS, and the Admin Portal.

AI agents should understand the deployment workflow before generating test plans, regression suites, automation, or release reports.

---

# Deployment Lifecycle

The standard deployment workflow follows the process below.

```

Business Requirement
│
▼
Requirement Analysis
│
▼
Design & Planning
│
▼
Development
│
▼
Code Review
│
▼
Pull Request Approval
│
▼
Merge into Development Branch
│
▼
Deploy to Development Environment
│
▼
Developer Verification
│
▼
Deploy to Staging Environment
│
▼
QA Functional Testing
│
▼
Regression Testing
│
▼
Business Validation (if required)
│
▼
QA Approval
│
▼
Production Approval
│
▼
Production Deployment
│
▼
Production Smoke Testing
│
▼
Release Completed

```

---

# Development Phase

Responsibilities

- Implement new features.
- Fix reported defects.
- Perform unit testing.
- Update documentation where required.
- Submit code for review.

Deliverables

- Source Code
- Pull Request
- Unit Test Results

---

# Code Review Phase

Objectives

- Verify coding standards.
- Review business logic.
- Identify potential regressions.
- Ensure maintainability.
- Validate implementation quality.

---

# Development Environment Validation

Verify

- Feature implementation
- Initial functionality
- Build stability
- Basic API functionality

---

# Staging Environment Validation

The Staging environment is the primary QA validation environment.

QA should perform:

- Functional Testing
- Regression Testing
- API Validation
- Cross-Platform Testing
- UI Validation
- Business Rule Verification
- Performance Observation
- Smoke Testing (where applicable)

---

# Production Validation

After deployment, QA should verify critical user journeys.

Examples

- Login
- Registration
- Wallet
- Payment
- Contest Join
- Draft
- Pick'em
- Notifications

Only production-safe verification should be performed.

---

# QA Approval Criteria

Before approving a release, verify:

- All planned features are implemented.
- Critical defects are resolved.
- Regression testing is completed.
- No blocker or critical issues remain.
- APIs function correctly.
- No application crashes occur.
- Release notes are reviewed.

---

# Release Checklist

Before Production Deployment

Verify:

- Feature implementation completed.
- Test cases executed.
- Regression completed.
- Build validated.
- High-priority defects resolved.
- Documentation updated.
- Required approvals received.

---

# Rollback Strategy

If a critical production issue is identified:

- Notify the development team immediately.
- Assess user impact.
- Follow the approved rollback process.
- Verify application stability after rollback.
- Perform production smoke testing after recovery.

---

# AI Agent Responsibilities

When assisting with release activities, AI agents should:

- Review release scope.
- Identify impacted business modules.
- Recommend regression coverage.
- Generate release validation checklists.
- Highlight integration risks.
- Generate production smoke test scenarios.
- Summarize release risks.

AI agents must never recommend production deployment without successful QA validation.

---

# Best Practices

Always:

- Test in Staging before Production.
- Validate business rules.
- Verify cross-platform consistency.
- Review release notes.
- Perform production smoke testing.
- Document release observations.

Never:

- Skip regression testing for impacted modules.
- Deploy unverified features.
- Ignore blocker defects.
- Perform destructive testing in Production.

---

# Related Documentation

- Development Environment
- Environment URLs
- Frontend QA Guidelines
- API QA Guidelines
- Reporting Format
- Release Notes

# 17. AI Responsibilities

## Overview

This repository is designed to enable AI agents to assist QA Engineers, Automation Engineers, Developers, Product Managers, and Business Analysts throughout the software development lifecycle.

AI agents should act as intelligent assistants by leveraging the documentation in this repository to generate accurate, maintainable, and business-compliant outputs.

AI should always prioritize documented business rules over assumptions and should request clarification whenever documentation is incomplete or ambiguous.

---

# Primary Responsibilities

AI agents are expected to assist with the following activities:

- Understanding business requirements
- Analyzing feature documentation
- Generating QA documentation
- Creating manual test cases
- Generating automation scripts
- Reviewing code changes
- Performing API analysis
- Identifying regressions
- Supporting release validation
- Creating technical documentation
- Assisting with defect analysis

---

# Documentation Analysis

AI agents should:

- Read AGENTS.md before performing any task.
- Review the relevant documentation under the `flows/` directory.
- Understand business workflows before generating outputs.
- Follow documented business rules.
- Reference related documentation whenever applicable.

AI should never generate outputs based solely on assumptions.

---

# Manual Testing Support

AI agents should assist by generating:

- Functional Test Cases
- Regression Test Cases
- Smoke Test Cases
- Exploratory Testing Ideas
- Cross-Platform Test Scenarios
- Positive Test Scenarios
- Negative Test Scenarios
- Boundary Value Test Cases
- Edge Case Scenarios

Generated test cases should align with documented business requirements.

---

# Automation Support

AI agents should assist with:

- Appium Automation
- Playwright Automation
- Cypress Automation
- API Automation
- Test Data Preparation
- Locator Suggestions
- Page Object Design
- Reusable Utility Functions

Automation should follow the project's coding standards and best practices.

---

# API Analysis

AI agents should:

- Review API documentation.
- Validate request and response structures.
- Suggest API test scenarios.
- Verify status codes.
- Identify missing validations.
- Detect potential security concerns.

---

# Defect Analysis

When analyzing reported issues, AI agents should:

- Review business rules.
- Analyze reproduction steps.
- Identify affected modules.
- Suggest possible root causes.
- Differentiate between UI, API, backend, and configuration issues.
- Recommend additional validation where appropriate.

---

# Regression Analysis

AI agents should:

- Identify impacted modules.
- Recommend regression coverage.
- Suggest additional validation areas.
- Highlight integration risks.
- Review related business workflows.

Regression recommendations should be based on documented dependencies.

---

# Documentation Support

AI agents should assist in:

- Creating new documentation.
- Updating existing documentation.
- Maintaining consistent formatting.
- Improving documentation clarity.
- Identifying outdated information.
- Linking related documentation.

Documentation should remain accurate and version controlled.

---

# Code Review Support

AI agents may assist by reviewing:

- Business logic
- Coding standards
- Naming conventions
- Error handling
- API usage
- Test coverage
- Maintainability
- Security considerations

AI recommendations should complement—not replace—human code reviews.

---

# Release Support

AI agents should assist with:

- Release readiness reviews
- Regression planning
- Smoke test planning
- Release note generation
- Risk assessment
- Post-release validation

---

# AI Decision-Making Principles

Before generating any output, AI agents should:

1. Understand the requested task.
2. Identify the affected business domain.
3. Review the relevant documentation.
4. Apply documented business rules.
5. Consider platform-specific behavior.
6. Validate assumptions.
7. Generate structured and maintainable output.

---

# Expected AI Outputs

AI agents may generate:

- Business Documentation
- Test Cases
- Automation Scripts
- API Test Cases
- Bug Reports
- Root Cause Analysis
- Regression Checklists
- Release Checklists
- Code Review Feedback
- Technical Documentation
- Risk Assessments

All outputs should follow the documentation standards defined in this repository.

---

# AI Limitations

AI agents should:

- Acknowledge uncertainty when documentation is incomplete.
- Request clarification instead of making assumptions.
- Avoid generating undocumented business logic.
- Clearly identify assumptions when necessary.

AI should support engineering decisions but should not replace human review and approval.

---

# Related Documentation

- AGENTS.md
- Business Rules
- Frontend QA Guidelines
- API QA Guidelines
- Deployment Workflow
- Safety Rules
- Reporting Format
- flows/
- automation/

# 18. Safety Rules

## Overview

Safety is a fundamental principle of the Drafters AI Documentation Repository.

All AI agents, QA engineers, automation engineers, and developers must follow these safety rules to protect production systems, customer data, and business operations.

AI-generated recommendations, automation scripts, and documentation should always prioritize security, reliability, and compliance.

---

# General Safety Principles

Always:

- Follow documented business rules.
- Use approved QA environments for testing.
- Protect sensitive information.
- Verify changes before execution.
- Follow the organization's deployment and approval process.
- Report potential risks before implementation.

Never:

- Assume undocumented business logic.
- Expose sensitive information.
- Perform destructive actions without authorization.
- Bypass security controls.
- Recommend unsafe practices.

---

# Production Environment Safety

Production is a live environment serving real users.

AI agents and team members must never:

- Modify production databases.
- Delete production data.
- Execute destructive SQL queries.
- Disable authentication or authorization.
- Perform load testing without approval.
- Use production accounts for testing.
- Execute experimental automation scripts.
- Modify production configurations without an approved deployment process.

Only production-safe validation activities such as smoke testing and critical functionality verification should be performed.

---

# Test Environment Safety

Always:

- Use approved QA or staging environments.
- Use designated QA accounts.
- Use approved test data.
- Reset test data only in non-production environments.
- Clearly identify the environment before testing.

Never:

- Mix production and test data.
- Use personal accounts for testing.
- Execute automation against production unless explicitly approved.

---

# Data Security

Sensitive information must never be stored in this repository.

Examples include:

- Production credentials
- API keys
- Authentication tokens
- Database passwords
- Secret keys
- Personally Identifiable Information (PII)
- Financial information

Sensitive data should always be managed through approved secure systems.

---

# Documentation Safety

Documentation should:

- Reflect the current application behavior.
- Avoid exposing confidential information.
- Clearly distinguish documented facts from assumptions.
- Be reviewed and updated whenever business rules change.

AI-generated documentation should never include confidential or proprietary information that is not intended for documentation.

---

# Automation Safety

Automation scripts should:

- Execute only approved test scenarios.
- Clean up test data where applicable.
- Avoid destructive operations.
- Use environment-specific configurations.
- Log execution details appropriately.

Automation should never:

- Hardcode credentials.
- Modify production data.
- Disable application safeguards.
- Bypass authentication mechanisms.

---

# AI Safety Guidelines

AI agents should:

- Follow documented workflows.
- Use repository documentation as the primary source of truth.
- Request clarification when documentation is incomplete.
- Clearly state assumptions when necessary.
- Recommend safe and maintainable solutions.
- Respect documented business rules.

AI agents should never:

- Invent undocumented business logic.
- Recommend bypassing security controls.
- Generate unsafe automation.
- Recommend direct production changes.
- Expose confidential information.

---

# Defect Reporting Safety

When reporting issues:

- Include only relevant technical information.
- Remove sensitive data from logs and screenshots.
- Do not expose user information.
- Verify reproduction steps before reporting.
- Clearly identify the affected environment.

---

# Approval Requirements

The following activities require appropriate approval:

- Production deployments
- Database modifications
- Configuration changes
- Performance testing on production
- Security-related changes
- Access to production systems

AI agents should recommend following the established approval process before these activities are performed.

---

# Best Practices

Always:

- Follow least-privilege access principles.
- Validate changes in staging before production.
- Keep documentation up to date.
- Protect user privacy.
- Follow organizational security policies.

Never:

- Store secrets in documentation.
- Share confidential information.
- Perform unauthorized operations.
- Ignore security warnings.
- Assume production behavior without verification.

---

# Related Documentation

- Development Environment
- Environment URLs
- Deployment Workflow
- AI Responsibilities
- Reporting Format

# 19. Reporting Format

## Overview

This section defines the standard reporting format for Quality Assurance activities performed within the Drafters platform.

Consistent reporting enables QA Engineers, Developers, Product Managers, Business Analysts, and AI agents to communicate testing results clearly, efficiently, and accurately.

All manual testing, automation execution, regression testing, smoke testing, API validation, and release verification should follow the reporting standards defined in this document.

---

# Reporting Objectives

Every report should:

- Clearly communicate the testing scope.
- Identify the environment and application version.
- Summarize test execution results.
- Highlight critical issues and risks.
- Provide sufficient evidence for reported defects.
- Support release decision making.

---

# Standard Report Structure

Every QA report should include the following sections:

## 1. Report Summary

Provide a brief overview of the testing activity.

Include:

- Testing objective
- Scope of testing
- Overall outcome

---

## 2. Environment Information

Document:

- Environment (Development / Staging / Production)
- Platform (Web / Android / iOS / Admin Portal)
- Build Version
- Device / Browser
- Test Date

---

## 3. Testing Scope

List the modules or features tested.

Examples:

- Authentication
- Wallet
- Finix Payment
- Contest
- Draft
- Pick'em
- Notifications

---

## 4. Test Execution Summary

Include:

- Total Test Cases Executed
- Passed
- Failed
- Blocked
- Not Executed

Where applicable, include automation execution statistics.

---

## 5. Defect Summary

For each reported defect include:

- Defect ID
- Module
- Severity
- Priority
- Status
- Short Description

Critical and blocker issues should be highlighted separately.

---

## 6. Observations

Document:

- UI observations
- Functional observations
- Performance observations
- Platform-specific differences
- Known limitations

---

## 7. Supporting Evidence

Attach relevant evidence whenever available:

- Screenshots
- Screen Recordings
- Browser Console Logs
- API Responses
- Network Logs
- Crash Logs

---

## 8. Risk Assessment

Highlight:

- Critical Risks
- Business Risks
- Regression Risks
- Release Risks

Provide recommendations where appropriate.

---

## 9. Recommendations

Examples:

- Ready for Production
- Ready after Minor Fixes
- Regression Required
- Additional Validation Required
- Not Recommended for Release

Clearly explain the reasoning behind the recommendation.

---

## 10. Overall Status

Select one of the following:

- ✅ Ready for Testing
- ✅ Testing Completed
- ✅ Ready for Release
- ⚠️ Needs Fixes
- ❌ Blocked
- ❌ Release Not Recommended

---

# Defect Reporting Guidelines

Every reported defect should include:

- Title
- Environment
- Platform
- Build Version
- Preconditions
- Steps to Reproduce
- Expected Result
- Actual Result
- Severity
- Priority
- Supporting Evidence

Defect reports should be reproducible and easy to understand.

---

# Automation Reporting

Automation execution reports should include:

- Test Suite Name
- Execution Time
- Total Tests
- Passed Tests
- Failed Tests
- Skipped Tests
- Failure Summary
- Execution Logs
- Screenshots (if applicable)

---

# AI Agent Responsibilities

When generating reports, AI agents should:

- Follow the standard reporting structure.
- Summarize findings objectively.
- Highlight critical issues first.
- Include supporting evidence when available.
- Avoid assumptions or unsupported conclusions.
- Clearly distinguish observations from confirmed defects.

AI-generated reports should be professional, concise, and actionable.

---

# Reporting Best Practices

Always:

- Use clear and professional language.
- Include accurate environment details.
- Attach supporting evidence.
- Verify reported issues before submission.
- Highlight business impact where applicable.

Never:

- Report unverified defects.
- Omit critical testing information.
- Include confidential or sensitive data.
- Make assumptions without evidence.

---

# Related Documentation

- Frontend QA Guidelines
- API QA Guidelines
- Logging Requirements
- Deployment Workflow
- Release Notes
- reports/

# 20. Known Limitations

## Overview

This section documents known limitations, expected behaviors, temporary workarounds, and platform-specific constraints within the Drafters platform.

The purpose of this section is to help QA Engineers, Developers, Product Managers, Business Analysts, and AI agents distinguish between known limitations and newly introduced defects.

Known limitations should be reviewed regularly and updated as the application evolves.

---

# Purpose

This section helps to:

- Prevent duplicate defect reporting.
- Reduce unnecessary investigation.
- Improve regression testing efficiency.
- Provide context for expected application behavior.
- Help AI agents identify existing limitations before reporting new issues.

---

# Known Limitation Categories

Known limitations may include:

- UI limitations
- Platform-specific behavior
- Third-party service limitations
- Performance limitations
- Temporary feature restrictions
- Browser compatibility issues
- Mobile device compatibility issues
- Configuration limitations

---

# Temporary Known Issues

Temporary issues that are already acknowledged by the development team should be documented with the following information:

Include:

- Module
- Description
- Affected Platform
- Environment
- Current Status
- Planned Resolution (if available)
- Reference (JIRA / Task ID)

Example

| Module | Issue | Platform | Status |
|---------|-------|----------|--------|
| Wallet | Example issue description | Web | Under Investigation |
| Draft | Example issue description | Android | In Progress |

---

# Platform-Specific Limitations

Some features may behave differently due to platform capabilities.

Examples include:

- Web-specific behavior
- Android-specific behavior
- iOS-specific behavior
- Admin Portal limitations

Platform differences should be documented separately in the relevant feature documentation.

---

# Third-Party Service Limitations

Certain platform features depend on external services.

Examples include:

- Payment Gateway
- Identity Verification (KYC)
- Push Notification Services
- Email Services

Temporary service outages or provider limitations should be documented before reporting application defects.

---

# Environment Limitations

Behavior may vary depending on the environment.

Examples:

- Development environment instability
- Staging environment test data limitations
- Feature flags enabled only in specific environments
- Mock services replacing production integrations

AI agents should verify the active environment before reporting issues.

# Performance Limitations

Document known performance constraints such as:

- Temporary slow API responses
- Large dataset loading delays
- Scheduled maintenance impacts
- Third-party response delays

Performance observations should be supported with evidence before creating new defect reports.

---

# Documentation Guidelines

Every known limitation should include:

- Feature or Module
- Description
- Affected Platform
- Affected Environment
- Severity
- Current Status
- Reference ID (if available)

When the limitation is resolved, the documentation should be updated accordingly.

---

# AI Agent Responsibilities

Before reporting a defect, AI agents should:

- Review this section for existing limitations.
- Check the relevant feature documentation.
- Verify whether the behavior is expected.
- Avoid reporting documented limitations as new issues.
- Clearly distinguish between known limitations and newly identified defects.

---

# Best Practices

Always:

- Keep the list of known limitations up to date.
- Reference related documentation where applicable.
- Include issue tracking references when available.
- Review limitations during regression testing.

Never:

- Treat documented limitations as new defects.
- Leave outdated limitations in the documentation after they are resolved.
- Assume all unexpected behavior is a new issue without verification.

---

# Related Documentation

- flows/
- troubleshooting/
- release-notes/
- Reporting Format
- Business Rules

# 21. Project-Specific Notes

## Overview

This section contains project-specific information that is unique to the Drafters platform and may not be evident from the source code alone.

It provides additional context for QA Engineers, Automation Engineers, Developers, Product Managers, Business Analysts, and AI agents to understand platform-specific workflows, integrations, business configurations, and operational practices.

This section should be reviewed and updated whenever significant business or technical changes are introduced.

---

# Platform Overview

Drafters is a fantasy sports platform that supports multiple contest formats across Web, Android, iOS, and the Admin Portal.

The platform includes:

- User Authentication
- Registration
- KYC Verification
- Wallet & Payments
- Fantasy Contest Lobby
- Draft Contests
- Pick'em
- Props
- Props Booster
- Best Ball
- Best Ball Survival
- Rankings
- Leaderboards
- Notifications
- Rewards
- Responsible Gaming
- Admin Portal

---

# Supported Platforms

The Drafters platform consists of:

- Web Application
- Android Application
- iOS Application
- Admin Portal
- Backend APIs

Unless documented otherwise, business functionality should remain consistent across supported platforms.

---

# Third-Party Integrations

The platform integrates with external services that support business functionality.

Examples include:

- Finix Payment Gateway
- PayPal
- KYC Verification Provider
- Push Notification Services
- Email Services
- Analytics & Monitoring Services

Integration behavior may vary between environments and should be documented in the relevant feature documentation.

---

# Feature Flags

Certain features may be controlled through feature flags or configuration settings.

Examples include:

- Contest availability
- Payment methods
- Responsible Gaming features
- Promotional campaigns
- Notification features
- Experimental functionality

AI agents should verify feature availability before generating automation or reporting defects.

---

# Business Configuration

Many platform behaviors are configurable through the Admin Portal.

Examples include:

- Contest Configuration
- Draft Configuration
- Pick'em Configuration
- Props Booster Configuration
- Payment Configuration
- Responsible Gaming Rules
- Promotional Campaigns
- Notification Settings

Configuration changes may affect application behavior without requiring code changes.

---

# Cross-Platform Consistency

The Drafters platform supports multiple client applications.

AI agents and QA engineers should verify consistency across:

- Business Logic
- User Experience
- API Behavior
- Validation Rules
- Calculations
- Error Messages
- Navigation Flow

Platform-specific differences should be documented when they are intentional.

---

# QA Documentation Standards

Every new feature should include documentation covering:

- Business Overview
- User Flow
- Business Rules
- Validation Rules
- Test Scenarios
- API Information
- Automation Strategy
- Platform Differences
- Known Issues
- Related Modules

All documentation should follow the standard templates maintained in this repository.

---

# AI Documentation Standards

AI agents should:

- Read AGENTS.md before performing tasks.
- Review the appropriate feature documentation.
- Follow documented business rules.
- Reference related modules.
- Generate reusable documentation.
- Maintain consistent formatting.
- Request clarification when documentation is incomplete.

---

# Repository Maintenance

This repository should be updated whenever:

- A new feature is released.
- Business rules change.
- APIs are modified.
- UI workflows are updated.
- Automation standards change.
- New integrations are introduced.
- Release processes change.

Maintaining current documentation ensures that AI-generated outputs remain accurate and aligned with the latest application behavior.

---

# Future Enhancements

As the Drafters platform evolves, this repository may be expanded to include:

- Detailed Architecture Documentation
- API Reference Documentation
- Automation Framework Guidelines
- Performance Testing Standards
- Security Testing Guidelines
- Accessibility Guidelines
- AI Prompt Library
- Release Playbooks
- Troubleshooting Guides
- Knowledge Base Articles

---

# Repository Vision

The long-term goal of this repository is to serve as the official knowledge base for the Drafters platform.

It should enable:

- Faster onboarding of new team members.
- Consistent QA practices.
- Standardized automation development.
- Improved collaboration between teams.
- AI-assisted software development and testing.
- Centralized project knowledge.
- Continuous documentation improvement.

---

# AI Agent Final Instructions

Before generating any output, AI agents should:

1. Read AGENTS.md.
2. Understand the requested task.
3. Identify the affected business domain.
4. Review the corresponding documentation.
5. Apply documented business rules.
6. Consider platform-specific behavior.
7. Follow QA and coding standards.
8. Generate clear, maintainable, and reusable outputs.
9. Avoid undocumented assumptions.
10. Recommend clarification whenever documentation is insufficient.

AI agents should treat this repository as the primary source of truth for the Drafters platform.

---

# Related Documentation

- README.md
- architecture/
- flows/
- api/
- automation/
- test-data/
- reports/
- troubleshooting/
- release-notes/
