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
