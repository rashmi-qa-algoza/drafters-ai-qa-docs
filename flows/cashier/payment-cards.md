# Payment Cards

> **Module:** Payment Cards (Add Card & Saved Cards)
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
4. Entry Points
5. User Flow
6. UI Screens
7. Add Card
8. Saved Cards
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

The Payment Cards module allows users to securely add, manage, and use payment cards for deposits within the Drafters application.

Users can add new Credit or Debit Cards, securely save them for future deposits, view all previously saved cards, and remove cards that are no longer required.

The module supports secure payment processing while reducing the need for users to repeatedly enter card information.

---

# 2. Business Purpose

The Payment Cards module is designed to:

- Add new payment cards.
- Securely save payment cards.
- Display saved payment cards.
- Allow users to reuse saved cards.
- Allow users to remove saved cards.
- Simplify future deposits.
- Improve payment experience.
- Support secure payment processing.

---

# 3. Preconditions

Before accessing Payment Cards:

- User account exists.
- User is logged in.
- KYC verification is completed.
- Internet connection is available.
- Deposit feature is enabled.

---

# 4. Entry Points

Users can access the Add Card functionality from different locations depending on the platform.

## Web

```text
Lobby
      │
      ▼
Wallet
      │
      ▼
Add Card
      │
      ▼
Add Card Screen
```

---

## Android

Users can access Add Card from:

- Wallet → Add Card

OR

```text
Deposit
      │
      ▼
Credit / Debit Card
      │
      ▼
Add Card
      │
      ▼
Add Card Screen
```

---

## iOS

Users can access Add Card from:

- Wallet → Add Card

OR

```text
Deposit
      │
      ▼
Credit / Debit Card
      │
      ▼
Add Card
      │
      ▼
Add Card Screen
```

---

# 5. User Flow

## Add New Card

```text
Wallet

      │

      ▼

Add Card

      │

      ▼

Enter Card Details

      │

      ▼

Google reCAPTCHA v3

      │

 ┌──────┴───────────────┐

 ▼                      ▼

Pass             Failed / Low Score

 │                      │

 ▼                      ▼

Save Card       Google reCAPTCHA v2

                       │

                       ▼

             User Completes Challenge

                       │

                       ▼

                  Save Card

                       │

                       ▼

Card Successfully Added

                       │

                       ▼

Displayed in Saved Cards
```

---

## Deposit Using Saved Card

```text
Wallet

      │

      ▼

Deposit

      │

      ▼

Credit / Debit Card

      │

      ▼

Select Saved Card

      │

      ▼

Enter Deposit Amount

      │

      ▼

Deposit

      │

      ▼

Payment Successful

      │

      ▼

Wallet Updated
```

---

## Delete Card

```text
Saved Cards

      │

      ▼

Select Card

      │

      ▼

Delete Card

      │

      ▼

Confirmation Popup

      │

      ▼

Confirm Delete

      │

      ▼

Card Removed
```

---

## Delete Multiple Cards

```text
Saved Cards

      │

      ▼

Select Multiple Cards

      │

      ▼

Delete

      │

      ▼

Confirmation Popup

      │

      ▼

Confirm

      │

      ▼

Selected Cards Removed
```

---

# 6. UI Screens

## 6.1 Add Card Screen

### Purpose

Allows users to securely add a new Credit or Debit Card.

### Components

| Field | Required | Description |
|---------|----------|-------------|
| Name on Card | Yes | Cardholder name |
| Card Number | Yes | Credit/Debit Card Number |
| Expiry Date | Yes | MM / YY |
| CVV | Yes | Card security code |
| ZIP / Postal Code | Yes | Billing ZIP Code |

### Buttons

- Save Card
- Cancel

---

## Security

When adding a new card:

- Google reCAPTCHA v3 is executed automatically.
- If reCAPTCHA v3 validation fails or returns a low confidence score, Google reCAPTCHA v2 challenge is displayed.
- Card is saved only after successful reCAPTCHA verification.

---

# 7. Add Card

The Add Card feature allows users to securely save a payment card.

Supported cards include:

- Visa
- Mastercard
- American Express (if supported)
- Discover (if supported)

### Behaviour

- User enters all required card details.
- Card information is validated.
- Google reCAPTCHA validation is performed.
- Card is securely stored.
- Newly added card immediately appears in Saved Cards.

---

# 8. Saved Cards

The Saved Cards section displays all previously saved payment cards.

### Information Displayed

Each saved card displays:

- Card Brand
- Masked Card Number
- Expiry Date
- Default Card Indicator (if applicable)

### Available Actions

- Select Card
- Deposit using selected card
- Delete Single Card
- Delete Multiple Cards

Users can manage their saved cards without re-entering card information during future deposits.

---
# 9. Business Rules

## General Rules

- Users must be authenticated before accessing Payment Cards.
- KYC verification must be completed before adding or using payment cards.
- Only supported Credit and Debit Cards can be added.
- Card information must pass all validation rules before being saved.
- Newly added cards become available immediately in the Saved Cards section.
- Saved cards can be used for future deposits.
- Card details are securely processed and stored by the configured payment provider.
- Sensitive card information must never be displayed in plain text.

---

## Add Card Rules

- Every new card addition requires Google reCAPTCHA verification.
- Google reCAPTCHA v3 is executed automatically.
- If reCAPTCHA v3 fails or returns a low confidence score, Google reCAPTCHA v2 challenge is displayed.
- Card is saved only after successful reCAPTCHA verification.
- Failed reCAPTCHA prevents the card from being added.

---

## Saved Card Rules

- Saved cards are displayed using masked card numbers.
- Users can select any saved card for deposits.
- Saved cards do not require reCAPTCHA during deposit.
- Deleted cards are immediately removed from the Saved Cards list.
- Deleted cards cannot be used for future deposits.

---

## Delete Card Rules

- Users may delete a single saved card.
- Users may delete multiple saved cards (if supported).
- Delete action requires user confirmation.
- Canceling the confirmation dialog does not remove the card(s).

---

# 10. Validation Rules

| Field | Validation |
|--------|------------|
| Name on Card | Required |
| Card Number | Required, valid card number |
| Expiry Date | Required, valid future date |
| CVV | Required |
| ZIP / Postal Code | Required |
| Google reCAPTCHA v3 | Executed automatically |
| Google reCAPTCHA v2 | Displayed if v3 validation fails |

---

# 11. Positive Scenarios

## Add Card

- Add a valid Visa card.
- Add a valid Mastercard.
- Add a valid American Express card (if supported).
- Add a valid Discover card (if supported).
- Add card from Wallet.
- Add card from Deposit screen (Android/iOS).
- Successfully complete reCAPTCHA v3.
- Successfully complete reCAPTCHA v2 after v3 fallback.
- Newly added card appears in Saved Cards.

---

## Saved Cards

- View all saved cards.
- Select a saved card for deposit.
- Deposit using a saved card.
- Verify no reCAPTCHA is displayed for saved cards.

---

## Delete Cards

- Delete a single saved card.
- Delete multiple saved cards.
- Cancel delete confirmation.
- Verify deleted cards are removed from the list.

---

# 12. Negative Scenarios

## Add Card

- Empty Name on Card.
- Empty Card Number.
- Empty Expiry Date.
- Empty CVV.
- Empty ZIP Code.
- Invalid Card Number.
- Invalid Expiry Date.
- Invalid CVV.
- Invalid ZIP Code.
- Unsupported card type.
- Network failure.
- Payment provider unavailable.
- Google reCAPTCHA validation failed.
- User closes Google reCAPTCHA v2 challenge.

---

## Saved Cards

- No saved cards available.
- Unable to load saved cards.
- Selecting an expired card (if applicable).

---

## Delete Cards

- Delete request fails.
- Network interruption during delete.
- Server error during delete.

---

# 13. Edge Cases

- Add the same card again (duplicate card handling).
- Refresh page while adding a card.
- Close application during Add Card.
- Session expires while adding a card.
- Slow network during card save.
- Multiple Save Card button clicks.
- Multiple Delete button clicks.
- Delete last remaining card.
- Delete multiple cards simultaneously.
- Payment provider timeout.
- Google reCAPTCHA service unavailable.
- Google reCAPTCHA v2 displayed after v3 failure.

---

# 14. Error Messages

| Scenario | Expected Result |
|----------|-----------------|
| Empty Card Number | Card Number is required |
| Invalid Card Number | Invalid Card Number |
| Empty Expiry Date | Expiry Date is required |
| Invalid Expiry Date | Invalid Expiry Date |
| Empty CVV | CVV is required |
| Invalid CVV | Invalid CVV |
| Empty ZIP Code | ZIP Code is required |
| Invalid ZIP Code | Invalid ZIP Code |
| Unsupported Card | Card type not supported |
| reCAPTCHA Failed | Verification failed. Please try again. |
| Network Failure | Unable to process request |
| Server Error | Something went wrong |
| Delete Failed | Unable to delete card |

Use production messages whenever possible.

---

# 15. Platform Differences

| Feature | Web | Android | iOS |
|----------|-----|----------|-----|
| Add Card from Wallet | Supported | Supported | Supported |
| Add Card from Deposit Screen | Not Supported | Supported | Supported |
| Saved Cards | Supported | Supported | Supported |
| Delete Single Card | Supported | Supported | Supported |
| Delete Multiple Cards | Supported (if available) | Supported (if available) | Supported (if available) |
| Google reCAPTCHA | Supported | Supported | Supported |

---

# 16. Admin Configuration

Administrators may configure:

## Card Management

- Enable / Disable Add Card.
- Enable / Disable Saved Cards.
- Supported Card Types.
- Maximum Saved Cards per User.
- Duplicate Card Handling.

---

## Security

- Google reCAPTCHA v3 configuration.
- Google reCAPTCHA v2 fallback configuration.
- Fraud detection rules.
- Card validation rules.

---

## Payment Provider

- Payment provider enable / disable.
- Sandbox / Production configuration.
- API credentials.
- Payment timeout.
- Retry configuration.

---

## Feature Flags

Administrators may control:

- Add Card feature.
- Saved Cards feature.
- Delete Card feature.
- Multiple Delete feature.
- Platform-specific availability.

---
# 17. Test Data

| Scenario | Test Data |
|----------|-----------|
| Valid Visa Card | Supported test Visa card |
| Valid Mastercard | Supported test Mastercard |
| Valid American Express | Supported test Amex card (if supported) |
| Valid Discover Card | Supported test Discover card (if supported) |
| Invalid Card Number | Random invalid card number |
| Expired Card | Card with expired expiry date |
| Invalid CVV | Incorrect CVV |
| Invalid ZIP Code | Invalid billing ZIP/Postal Code |
| New User | No saved payment cards |
| Existing User | One or more saved cards |
| Multiple Saved Cards | Multiple valid saved cards |
| Duplicate Card | Previously saved card |

> **Note:** Never commit real payment card information to the repository. Use sandbox or test card data only.

---

# 18. Automation Strategy

Recommended automation coverage:

## UI Automation

- Open Add Card screen.
- Validate mandatory fields.
- Validate card number.
- Validate expiry date.
- Validate CVV.
- Validate ZIP / Postal Code.
- Verify Google reCAPTCHA v3 execution.
- Verify Google reCAPTCHA v2 fallback.
- Successfully add a new card.
- Verify newly added card appears in Saved Cards.
- Select a saved card for deposit.
- Delete a single saved card.
- Delete multiple saved cards.
- Verify delete confirmation popup.
- Verify cancel delete action.
- Verify Saved Cards list refresh.

---

## API Automation

- Add Card API
- Retrieve Saved Cards API
- Delete Card API
- Card Tokenization API (if exposed)
- Payment Provider API Integration

---

## Regression

Verify across:

- Web
- Android
- iOS

Recommended Frameworks:

- Playwright
- Appium

---

# 19. AI Implementation

## Automation Priority

High

## AI Tasks

AI should be able to:

- Generate Add Card automation.
- Generate Saved Cards automation.
- Generate Delete Card automation.
- Generate reCAPTCHA validation scenarios.
- Generate Payment Card regression suite.
- Generate API automation.
- Review Payment Card business rules.

## Recommended Prompts

Generate Playwright automation for Add Card.

Generate Appium automation for Saved Cards.

Generate Delete Card automation.

Generate Payment Cards regression suite.

Generate API tests for Payment Cards.

Review Payment Card validation rules.

---

# 20. Dependencies

Payment Cards depends on:

- Authentication
- KYC Verification
- Wallet
- Deposit
- Payment Gateway
- Google reCAPTCHA
- User Profile

---

# 21. Security Considerations

- HTTPS communication is mandatory.
- Card data must be securely tokenized.
- Card numbers must never be stored or displayed in plain text.
- Display only masked card numbers.
- Google reCAPTCHA protects Add Card requests.
- reCAPTCHA v3 executes automatically.
- reCAPTCHA v2 challenge is displayed when required.
- Secure user authentication is required before card management.
- Prevent unauthorized access to saved cards.
- Sensitive payment information must comply with PCI DSS requirements.

---

# 22. Performance Considerations

- Add Card screen should load within acceptable response time.
- Saved Cards should load quickly.
- Newly added cards should appear immediately after successful save.
- Deleted cards should disappear immediately after successful deletion.
- Card selection should update without unnecessary delays.
- Payment provider timeouts should be handled gracefully.

---

# 23. Accessibility Considerations

Verify:

- Keyboard navigation.
- Screen reader compatibility.
- Focus order.
- Form labels.
- Accessible validation messages.
- Accessible confirmation dialogs.
- Color contrast.
- Readable masked card information.

---

# 24. Related Modules

- Authentication
- KYC
- Wallet
- Deposit
- Cash Out
- Account History

---

# 25. Known Issues

Document current issues affecting Payment Cards.

Examples:

- Payment provider issues.
- Platform-specific UI inconsistencies.
- Card validation issues.
- Saved Card synchronization issues.

Leave blank if none exist.

---

# 26. Future Enhancements

Document only confirmed product roadmap items.

Examples:

- Default payment card selection.
- Card nickname support.
- Card expiration notifications.
- Additional card brands.
- Regional payment methods.
- Improved payment card management.

Avoid documenting speculative enhancements.

---

# 27. Related Documentation

- AGENTS.md
- README.md
- architecture/system-overview.md
- flows/wallet.md
- flows/deposit.md
- flows/account-history.md
- flows/cash-out.md
- api/payment-cards-api.md

---

# 28. Revision History

| Version | Date | Author | Description |
|----------|------|--------|-------------|
| 1.0 | YYYY-MM-DD | QA Team | Initial Version |

---
