# Deposit

> **Module:** Deposit
>
> **Application:** Drafters Fantasy Sports
>
> **Platforms:** Web | Android | iOS
>
> **Business Owner:** Product Team
>
> **Technical Owner:** Engineering Team
>
> **QA Owner:** QA Team
>
> **Status:** Active
>
> **Version:** 1.0
>
> **Last Updated:** YYYY-MM-DD

---

# Table of Contents

1. Overview
2. Business Purpose
3. Preconditions
4. User Flow
5. Entry Points
6. UI Screens
7. Payment Methods
8. Promo Code
9. Business Rules
10. Validation Rules
11. Positive Scenarios
12. Negative Scenarios
13. Edge Cases
14. Error Messages
15. Platform Differences
16. Admin Configuration
17. Test Data
18. Automation Strategy
19. AI Implementation
20. Dependencies
21. Security Considerations
22. Performance Considerations
23. Accessibility Considerations
24. Related Modules
25. Known Issues
26. Future Enhancements
27. Related Documentation
28. Revision History

---

# 1. Overview

## Description

The Deposit module allows verified users to securely add funds to their Drafters wallet using supported payment methods.

After KYC verification, users can deposit funds to participate in paid Draft contests, Pick'em contests, and other real-money games.

First-time users receive a Welcome Deposit experience with an eligible promotional code, while existing users can deposit normally with optional promo code support.

Successful deposits immediately update the user's wallet balance and create an Account History transaction.

---

# 2. Business Purpose

The Deposit module is designed to:

- Allow users to add funds securely.
- Support multiple payment methods.
- Support promotional bonus campaigns.
- Apply first-time deposit promotions.
- Update Cash Balance immediately.
- Update Bonus Balance when applicable.
- Record all deposits in Account History.
- Enable participation in paid contests.

---

# 3. Preconditions

Before making a deposit:

- User account exists.
- User is logged in.
- KYC verification is completed.
- User satisfies minimum age requirements.
- Internet connection is available.
- Payment gateway is operational.

---

# 4. User Flow

## First-Time User

```text
Registration
      │
      ▼
Login
      │
      ▼
KYC Verification
      │
      ▼
Lobby
      │
      ▼
Welcome Deposit Banner
      │
      ▼
Click "Deposit Now"
      │
      ▼
Welcome Deposit Screen
      │
      ▼
Default Promo Applied
      │
      ▼
Select Deposit Amount
      │
      ▼
Select Payment Method
      │
      ▼
Complete Payment
      │
      ▼
Deposit Successful
      │
      ▼
Cash Balance Updated
      │
      ▼
Bonus Applied
      │
      ▼
Account History Updated
      │
      ▼
Welcome Banner Removed
```

---

## Existing User

```text
Lobby
      │
      ▼
Click Deposit
      │
      ▼
Cashier
      │
      ▼
Summary
      │
      ▼
Add Funds
      │
      ▼
Choose Payment Method
      │
      ▼
Enter Deposit Details
      │
      ▼
Deposit Successful
      │
      ▼
Wallet Updated
```

---

# 5. Entry Points

Users can access Deposit from multiple locations.

## First-Time User

- Welcome Deposit Banner
- Deposit button
- Wallet Balance
- Cashier → Summary → Add Funds

## Existing User

- Deposit button
- Wallet Balance
- Cashier → Summary → Add Funds

## Insufficient Balance

When attempting:

- Join Paid Draft Contest
- Join Paid League
- Create Pick'em Entry

If the user has insufficient funds, an **Insufficient Balance** message is displayed, allowing the user to navigate to the Deposit flow.

---

# 6. UI Screens

## 6.1 Welcome Deposit Screen (First-Time Users)

Displayed after successful KYC verification when the user clicks **Deposit Now** from the Welcome Deposit banner.

### Components

- Welcome Bonus Banner
- Promo Code field (pre-filled with default Welcome Promo)
- Deposit Amount field
- Preset Amount buttons ($25, $50, $100, $500)
- Payment Method buttons
- Skip and Go To Lobby

---

## 6.2 Cashier Summary

Accessible from:

- Deposit button
- Wallet Balance
- Cashier

Displays:

- Cash Balance
- Bonus Balance
- Available To Play
- In Play
- Currently Winning
- Tickets
- Add Funds button

Clicking **Add Funds** opens the Deposit flow.

---

## 6.3 Payment Method Selection

After clicking **Add Funds**, users can choose a payment method.

### Web

- PayPal
- Credit / Debit Card

### Android

- PayPal
- Credit / Debit Card

### iOS

- PayPal
- Apple Pay
- Credit / Debit Card

---

## 6.4 PayPal Deposit Screen

### Components

- Deposit Amount
- Preset Amount buttons
- Promo Code
- Apply Promo button
- PayPal button

### Behaviour

- User selects amount.
- User may apply a promo code.
- Clicking **PayPal** redirects to the PayPal payment gateway.
- After successful authorization, the user returns to Drafters and the deposit is completed.

---

## 6.5 Apple Pay Deposit Screen (iOS)

### Components

- Deposit Amount
- Preset Amount buttons
- Promo Code
- Apply Promo button
- Apple Pay button

### Behaviour

- Available only on iOS supported devices.
- User authorizes payment using Apple Pay.
- After successful authorization, deposit is completed.

---

## 6.6 Credit / Debit Card Deposit Screen

### Components

- Deposit Amount
- Preset Amount buttons
- Promo Code
- Apply button
- Name on Card
- Card Number
- Expiry Date
- CVV
- Zip / Postal Code
- Deposit button

### Behaviour

- User enters card details.
- Promo code is validated.
- Clicking **Deposit** initiates payment processing.

For the first card addition:

- Invisible reCAPTCHA v3 is executed.
- If reCAPTCHA v3 validation fails, reCAPTCHA v2 challenge is displayed.
- Deposit proceeds only after successful reCAPTCHA verification.

For saved cards:

- Saved card details are used.
- No reCAPTCHA challenge is displayed.

# 7. Payment Methods

## PayPal

Supported Platforms

- Web
- Android
- iOS

Flow

1. Select PayPal.
2. Choose Deposit Amount.
3. Apply Promo Code (optional).
4. Redirect to PayPal.
5. Authenticate payment.
6. Return to Drafters.
7. Wallet updated.

---

## Apple Pay

Supported Platform

- iOS only

Flow

1. Select Apple Pay.
2. Choose Deposit Amount.
3. Apply Promo Code (optional).
4. Complete Apple Pay authorization.
5. Wallet updated.

---

## Credit / Debit Card

Supported Platforms

- Web
- Android
- iOS

Flow

1. Choose Deposit Amount.
2. Enter Promo Code (optional).
3. Enter Card Details.
4. Complete reCAPTCHA (first card only).
5. Submit Deposit.
6. Payment processed.
7. Wallet updated.

For saved cards:

- Card details are auto-filled.
- User selects saved card.
- reCAPTCHA is not required.

# 8. Promo Code

## First-Time User

- Default promo code is automatically applied.
- User may remove the promo code.
- User may replace it with another valid promo.
- Promo validation occurs before payment.
- After the first successful deposit, the default promo cannot be used again.

---

## Existing User

- Promo field is empty.
- User may manually enter a valid promo code.
- Invalid promo codes display validation errors.
- Valid promo updates eligible bonus.

---

# 9. Business Rules

- Deposit is allowed only after successful KYC verification.
- Users must be eligible for real-money gameplay.
- Deposit requires a supported payment method.
- Deposit amount must satisfy configured minimum and maximum limits.
- Promo codes are validated before payment.
- Default Welcome Promo is available only for eligible first-time users.
- Welcome Promo cannot be reused after successful redemption.
- Successful deposits update Cash Balance immediately.
- Bonus Balance updates according to the applied promotion.
- Every successful deposit creates an Account History entry.
- Welcome Deposit Banner disappears after the first successful deposit.
- Users with insufficient wallet balance are prompted to deposit before joining paid contests.

## Deposit Amount

- User may enter a custom amount.
- User may select preset deposit amounts.
- Custom amount must satisfy configured minimum and maximum limits.

## Payment Methods

- Available payment methods depend on platform.
- Apple Pay is available only on supported iOS devices.
- Unsupported payment methods are hidden.

## Credit / Debit Card

- New card requires all mandatory fields.
- Saved cards may be reused.
- First-time card addition requires reCAPTCHA validation.
- Saved cards do not require reCAPTCHA.

## PayPal

- Deposit completes only after successful PayPal authorization.

## Apple Pay

- Deposit completes only after successful Apple Pay authorization.

---

# 10. Validation Rules

| Field | Validation |
|--------|------------|
| Deposit Amount | Required |
| Promo Code | Optional |
| Name on Card | Required |
| Card Number | Required |
| Expiry Date | Required |
| CVV | Required |
| Zip Code | Required |
| Payment Method | Required |
| PayPal Authorization | Required |
| Apple Pay Authorization | Required |
| reCAPTCHA v3 | Executed for first card addition |
| reCAPTCHA v2 | Displayed if v3 validation fails |

---

# 11. Positive Scenarios

- First deposit using default promo.
- First deposit after changing promo.
- Existing user deposit.
- Deposit using PayPal.
- Deposit using Credit Card.
- Deposit using Apple Pay.
- Valid promo applied.
- Wallet balance updates correctly.
- Bonus balance updates correctly.
- Account History entry created.
- Welcome Banner disappears after first successful deposit.
- Deposit using custom amount.
- Deposit using preset amount.
- Deposit with saved card.
- Deposit with newly added card.
- Deposit after successful reCAPTCHA v3.
- Deposit after reCAPTCHA v2 fallback.
- Successful PayPal authorization.
- Successful Apple Pay authorization.

---

# 12. Negative Scenarios

- Empty deposit amount.
- Deposit below minimum amount.
- Deposit above maximum amount.
- Invalid promo code.
- Expired promo code.
- Already used promo code.
- Payment declined.
- Payment cancelled.
- Network interruption.
- Server unavailable.
- Payment gateway failure.
- Unsupported payment method.
- Attempt to reuse first deposit promo.
- Empty card number.
- Invalid card number.
- Invalid CVV.
- Invalid expiry date.
- Invalid ZIP code.
- PayPal authorization cancelled.
- Apple Pay authorization cancelled.
- reCAPTCHA validation failed.
- Payment gateway timeout.

---

# 13. Edge Cases

- Multiple Deposit button clicks.
- Browser refresh during payment.
- App closed during payment.
- Payment timeout.
- Duplicate payment attempt.
- Promo removed before payment.
- Promo changed before payment.
- Switching payment methods.
- Slow network.
- Payment succeeds but response delayed.
- Switch payment method before deposit.
- Change promo after amount selection.
- Remove promo before payment.
- Add multiple saved cards.
- Payment succeeds after retry.
- Payment gateway callback delayed.

---

# 14. Error Messages

| Scenario | Expected Result |
|----------|-----------------|
| Empty Amount | Deposit amount is required |
| Invalid Promo | Promo code is invalid |
| Expired Promo | Promo code has expired |
| Promo Already Used | Promo code already redeemed |
| Payment Failed | Deposit failed |
| Payment Cancelled | Payment cancelled |
| Payment Declined | Payment declined |
| Network Failure | Unable to process request |
| Server Error | Something went wrong |
| Insufficient Balance | Insufficient balance |
| Invalid Card | Invalid card details |
| Invalid CVV | Invalid CVV |
| Invalid Expiry | Invalid expiry date |
| Invalid ZIP | Invalid ZIP code |
| reCAPTCHA Failed | Verification failed. Please try again. |
| PayPal Cancelled | Payment cancelled |
| Apple Pay Cancelled | Payment cancelled |

Use production messages whenever possible.

---

# 15. Platform Differences

| Feature | Web | Android | iOS |
|----------|-----|----------|-----|
| Welcome Deposit Screen | Yes | Yes | Yes |
| Default Promo (First Deposit) | Yes | Yes | Yes |
| PayPal | Yes | Yes | Yes |
| Credit / Debit Card | Yes | Yes | Yes |
| Apple Pay | No | No | Yes |
| Skip and Go To Lobby | Yes | Yes | Yes |
| Cashier | Yes | Yes | Yes |

---

# 16. Admin Configuration

Deposit behavior may be configured through:

- Minimum Deposit Amount
- Maximum Deposit Amount
- Default Deposit Amount
- Welcome Deposit Promotion
- Promo Code Management
- Bonus Percentage
- Eligible User Rules
- Payment Method Enable/Disable
- Country Restrictions
- Platform-specific Payment Methods
- Payment Gateway Configuration
- Deposit Limits (Daily / Weekly / Monthly)
- Responsible Gaming Settings
- Feature Flags

# 17. Test Data

| Scenario | Test Data |
|----------|-----------|
| First-Time User | Verified account eligible for Welcome Deposit |
| Existing User | Verified account with previous deposit |
| Valid Promo Code | Active promotional code |
| Invalid Promo Code | Random invalid code |
| Expired Promo Code | Expired promotional code |
| Used Promo Code | Previously redeemed code |
| Minimum Deposit | Configured minimum amount |
| Maximum Deposit | Configured maximum amount |
| Valid Credit Card | Supported test card |
| Valid PayPal Account | Sandbox/Test PayPal account |
| Apple Pay | Supported iOS device with Apple Pay configured |

Sensitive payment credentials should never be committed to the repository.

---

# 18. Automation Strategy

Recommended automation coverage:

### UI Automation

- Welcome Deposit flow
- Existing User Deposit flow
- Deposit amount selection
- Promo code validation
- Payment method selection
- Wallet balance verification
- Bonus balance verification
- Account History verification
- First Deposit Banner removal
- Cashier navigation

### API Automation

- Deposit API
- Promo Code Validation API
- Wallet API
- Account History API

### Regression

- Web
- Android
- iOS
- Cross-browser
- Responsive UI

Recommended Frameworks:

- Playwright
- Appium

---

# 19. AI Implementation

## Automation Priority

High

## AI Tasks

AI should be able to:

- Generate Deposit automation.
- Generate Wallet verification automation.
- Generate Promo Code validation tests.
- Generate Account History validation.
- Generate Deposit API tests.
- Generate regression scenarios.
- Review Deposit business rules.

## Recommended Prompts

Generate Playwright automation for Deposit.

Generate Appium automation for Deposit.

Generate Deposit API tests.

Generate Wallet verification tests.

Generate Deposit regression suite.

Review Deposit business rules.

---

# 20. Dependencies

Deposit depends on:

- Authentication
- KYC Verification
- Wallet
- Promo Code Service
- Payment Gateway
- Account History
- Responsible Gaming
- User Profile

---

# 21. Security Considerations

- HTTPS communication.
- Secure payment gateway integration.
- PCI-compliant payment processing.
- Sensitive payment information must not be stored in plain text.
- Promo code validation should be performed server-side.
- Prevent duplicate deposit requests.
- Secure session validation before payment.
- Fraud prevention checks.
- Deposit limits based on Responsible Gaming settings.

---

# 22. Performance Considerations

- Deposit screen should load quickly.
- Payment processing should complete within acceptable response time.
- Wallet balance should update immediately after successful payment.
- Bonus calculation should be applied without noticeable delay.
- Account History should be updated immediately.
- Duplicate payment requests should be prevented.

---

# 23. Accessibility Considerations

Verify:

- Keyboard navigation.
- Screen reader compatibility.
- Focus order.
- Form labels.
- Validation accessibility.
- Button accessibility.
- Color contrast.
- Error message readability.

---

# 24. Related Modules

- Authentication
- Registration
- KYC
- Wallet
- Cashier
- Promo Code
- Account History
- Responsible Gaming
- Draft
- Pick'em
- Contest Join
- Cash Out

---

# 25. Known Issues

Document current known issues affecting the Deposit module.

Examples:

- Payment gateway issues.
- Platform-specific UI differences.
- Promo code validation issues.
- Wallet synchronization issues.

Leave blank if none exist.


# 27. Related Documentation

- AGENTS.md
- README.md
- architecture/system-overview.md
- flows/authentication.md
- flows/registration.md
- flows/kyc.md
- flows/wallet.md
- flows/cashier.md
- flows/account-history.md
- api/deposit-api.md
- api/promo-api.md
- api/wallet-api.md

---

# 28. Revision History

| Version | Date | Author | Description |
|----------|------|--------|-------------|
| 1.0 | YYYY-MM-DD | QA Team | Initial Version |
