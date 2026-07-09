# Drafters Mobile Architecture

> **Document:** Mobile Architecture
>
> **Version:** 1.0
>
> **Platforms:** Android | iOS

---

# Table of Contents

1. Overview
2. Purpose
3. Mobile Applications
4. Architecture
5. Shared Features
6. Platform Differences
7. API Communication
8. Notifications
9. Payments
10. QA Considerations
11. AI Context
12. Related Documentation
13. Revision History

---

# 1. Overview

The Drafters mobile applications provide native Android and iOS experiences while sharing common backend services and business functionality.

---

# 2. Purpose

Explain how Android and iOS applications are structured and interact with backend services.

---

# 3. Mobile Applications

- Android
- iOS

Both platforms support:

- Authentication
- Wallet
- Draft
- Pick'em
- Rankings
- Notifications
- Responsible Gaming

---

# 4. Architecture

```text
User
   │
   ▼
Android / iOS
   │
   ▼
REST APIs
   │
   ▼
Backend Services
   │
   ▼
Database
```

---

# 5. Shared Features

- Authentication
- Wallet
- Contest
- Draft
- Pick'em
- Notifications

---

# 6. Platform Differences

Examples include:

- Native UI Components
- Device Permissions
- Push Notification Handling
- Payment SDK Integration

Business rules remain consistent across platforms.

---

# 7. API Communication

Mobile applications communicate using secure REST APIs.

---

# 8. Notifications

Supports:

- Push Notifications
- In-App Notifications

---

# 9. Payments

Supports:

- Finix
- PayPal

Payment processing follows backend business rules.

---

# 10. QA Considerations

Validate:

- Cross-platform consistency
- UI behavior
- API responses
- Device compatibility
- Offline scenarios

---

# 11. AI Context

AI agents should use this document when generating:

- Appium automation
- Mobile regression suites
- Cross-platform validation
- Mobile bug analysis

---

# 12. Related Documentation

- frontend-architecture.md
- backend-architecture.md
- flows/

---

# 13. Revision History

| Version | Date | Author | Description |
|----------|------|--------|-------------|
| 1.0 | | QA Team | Initial Version |
