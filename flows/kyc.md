# Know Your Customer (KYC)

> **Module:** KYC Verification
>
> **Application:** Drafters Fantasy Sports
>
> **Platforms:** Web | Android | iOS
>
> **Status:** Active
>
> **Version:** 1.0

---

# Table of Contents

1. Overview
2. Business Purpose
3. Preconditions
4. User Journey
5. User Flow
6. Verification Entry Points
7. Verification Process
8. Business Rules
9. Validation Rules
10. Positive Scenarios
11. Negative Scenarios
12. Edge Cases
13. Platform Behaviour
14. Test Scenarios
15. Automation Strategy
16. AI Implementation
17. Dependencies
18. Related Documents

---

# 1. Overview

## Description

The KYC (Know Your Customer) module verifies a user's identity before allowing access to regulated fantasy sports features.

Drafters is a US and Canada based Daily Fantasy Sports application. Due to legal and financial regulations, users must successfully complete identity verification before participating in paid contests or performing financial transactions.

Users can explore the application before completing KYC, but important gameplay and wallet features remain restricted.

---

# 2. Business Purpose

KYC verification ensures:

- Identity verification
- Age verification (18+)
- Regulatory compliance
- Fraud prevention
- Financial security
- Location eligibility
- Safe participation in paid fantasy contests

---

# 3. Preconditions

Before starting KYC:

- User account is registered.
- Phone number is verified.
- User is logged in.
- User reaches the Lobby screen.
- Internet connection is available.

---

# 4. User Journey

```text
Landing Page
      │
      ▼
Registration
      │
      ▼
OTP Verification
      │
      ▼
Login
      │
      ▼
Lobby
      │
      ▼
User can browse application

      │
      ▼
Attempts any restricted feature

      │
      ▼
KYC Verification Required

      │
      ▼
Identity Verification

      │
      ▼
Verification Successful

      │
      ▼
Full Platform Access
```

---

# 5. User Flow

```text
User Login

      │

      ▼

Lobby Screen

      │

      ├───────────────► Click "Verify Your Account Here"

      │

      ├───────────────► Click Wallet Balance

      │

      ├───────────────► Click Add Funds (+)

      │

      ├───────────────► Join Draft Contest

      │

      ├───────────────► Create Pick'em Entry

      │

      └───────────────► Any Restricted Feature

                       │

                       ▼

             Verification Required Popup

                       │

                       ▼

                   Click OK

                       │

                       ▼

              Verify Your Account Screen

                       │

                       ▼

          Start Verification

                       │

                       ▼

      Step 1: Document Verification

                       │

                       ▼

      Step 2: Selfie Verification

                       │

                       ▼

         Identity Verification

                       │

              ┌───────────────┐

              ▼               ▼

         Approved         Failed

              │               │

              ▼               ▼

    Features Enabled     Retry Verification
```

---

# 6. Verification Entry Points

Users can start KYC from multiple locations.

### Lobby Banner

A verification banner is displayed at the top of the Lobby.

```
Verify Your Account To Enter Real Money Contests
Verify Your Account Here
```

Clicking the banner redirects to the KYC screen.

---

### Wallet Balance

Selecting the wallet balance redirects the user to verification if KYC is incomplete.

---

### Add Funds (+)

Attempting to add funds requires KYC.

---

### Join Draft Contest

Joining paid contests requires successful verification.

---

### Pick'em Entry

Creating a Pick'em ticket requires successful verification.

---

### Wallet Actions

The following wallet options require KYC:

- Add Funds
- Add Card
- Cashout
- Saved Cards

---

# 7. Verification Process

The verification screen explains the complete identity verification process.

## Step 1

Document Verification

Supported documents include:

- Driver's License
- Passport
- National ID Card

---

## Step 2

Selfie Verification

The user captures a live selfie.

The system compares the selfie against the uploaded identity document.

---

## Photo Guidelines

Users are instructed to:

- Keep entire face visible.
- Remove objects covering the face.
- Use proper lighting.
- Capture clear document images.
- Fit document completely inside the frame.
- Avoid blurry images.

---

# 8. Business Rules

- User must be at least 18 years old.
- KYC is mandatory before participating in paid fantasy contests.
- Users may browse the application without verification.
- Users cannot access regulated features until KYC is approved.
- Verification status is shared across Web, Android, and iOS.
- Identity verification consists of:
  - Document Verification
  - Selfie Verification
- Verification is completed through the integrated identity verification provider.

---

# 9. Validation Rules

Verify:

- Valid identity document.
- Clear document image.
- Complete document inside capture frame.
- Face clearly visible.
- Successful selfie capture.
- Identity match between document and selfie.

---

# 10. Positive Scenarios

- User opens KYC from Lobby banner.
- User starts verification from Wallet.
- User uploads valid document.
- Selfie matches identity.
- Verification approved.
- Wallet features unlocked.
- Deposit enabled.
- Contest joining enabled.
- Pick'em enabled.

---

# 11. Negative Scenarios

- Invalid identity document.
- Blurry document.
- Face not detected.
- Selfie mismatch.
- Verification cancelled.
- Camera permission denied.
- Network failure.
- Verification timeout.

---

# 12. Edge Cases

- User exits during verification.
- Camera closes unexpectedly.
- Internet disconnects.
- User retries verification.
- Duplicate verification attempt.
- Verification provider unavailable.

---

# 13. Platform Behaviour

## Web

- Verification available.
- Same business rules apply.

## Android

- Lobby banner displayed.
- Wallet restrictions enforced.
- Camera used for document and selfie capture.

## iOS

- Same behaviour as Android.
- Same verification process.

---

# 14. Test Scenarios

Functional Testing

- Verify Lobby banner.
- Verify restricted features redirect to KYC.
- Verify popup behaviour.
- Verify Start Verification.
- Verify document capture.
- Verify selfie capture.
- Verify successful verification.
- Verify rejected verification.
- Verify retry flow.
- Verify Wallet unlock.
- Verify Draft contest access.
- Verify Pick'em access.

Regression

- Existing verified user.
- Existing unverified user.
- Cross-platform verification.
- Wallet restrictions.
- Contest restrictions.

---

# 15. Automation Strategy

Recommended automation coverage:

UI

- Lobby banner
- Wallet redirect
- Verification popup
- KYC flow
- Verification success
- Feature unlock

API

- Verification API
- Verification status API

Frameworks

- Playwright
- Appium

---

# 16. AI Implementation

AI should be able to:

- Generate Playwright tests.
- Generate Appium tests.
- Generate KYC regression suite.
- Validate business rules.
- Generate edge-case scenarios.
- Verify feature restrictions for unverified users.

---

# 17. Dependencies

Registration

Authentication

OTP Verification

Wallet

Contest

Pick'em

Responsible Gaming

Identity Verification Provider

---

# 18. Related Documents

flows/registration.md

flows/authentication.md

flows/wallet.md

flows/responsible-gaming.md

api/identity-verification.md

AGENTS.md
