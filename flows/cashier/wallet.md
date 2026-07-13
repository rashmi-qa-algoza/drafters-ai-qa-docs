# Wallet (Cashier)

> **Module:** Wallet (Cashier)
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
6. Wallet Navigation
7. Wallet Summary
8. Wallet Sections
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

The Wallet (Cashier) module is the central financial hub of the Drafters application.

It allows users to view wallet balances, access deposit and withdrawal features, manage saved payment methods, review transaction history, view promotional tickets, and access available offers.

The Wallet does not perform financial transactions directly. Instead, it provides navigation to the appropriate financial modules.

---

# 2. Business Purpose

The Wallet module is designed to:

- Display account balances.
- Display available contest balance.
- Display active contest balance.
- Display current winnings.
- Display available tickets.
- Provide access to Deposit.
- Provide access to Cash Out.
- Provide access to Account History.
- Provide access to Saved Cards.
- Provide access to Offers.
- Provide access to Verification.

---

# 3. Preconditions

Before accessing Wallet:

- User account exists.
- User is logged in.
- Internet connection is available.

Some wallet features require:

- Successful KYC Verification.
- Eligible account.
- Supported payment method.

---

# 4. User Flow

```text
Login
      │
      ▼
Lobby
      │
      ▼
Click Wallet Balance
      │
      ▼
Wallet (Cashier)
      │
      ▼
Summary Screen
      │
      ├────────► Add Funds
      │
      ├────────► Add A Card
      │
      ├────────► Saved Cards
      │
      ├────────► Cash Out
      │
      ├────────► Account History
      │
      ├────────► Tickets
      │
      └────────► Offers
```

---

# 5. Entry Points

Users can open the Wallet from:

- Wallet Balance displayed in Lobby.
- Deposit Success flow.
- Navigation Menu.
- Account Menu.

---

# 6. Wallet Navigation

The Wallet contains the following navigation menu:

- Summary
- Add Funds
- Add A Card
- Saved Cards
- Cash Out
- Account History
- Tickets
- Offers

Each menu opens its respective module.

---

# 7. Wallet Summary

The Summary screen is the default landing page of the Wallet.

It displays an overview of the user's financial account.

### Summary Information

| Field | Description |
|--------|-------------|
| Cash Balance | Total available cash balance in the wallet. |
| Bonus Balance | Promotional bonus available for eligible contests. |
| Available To Play | Total amount available to join contests (Cash + Eligible Bonus). |
| In Play | Amount currently used in active contests. |
| Currently Winning | Live winnings from contests that have not yet settled. |
| Tickets | Total available promotional tickets. |

### Action Button

- Add Funds

Selecting **Add Funds** redirects the user to the Deposit module.

---

# 8. Wallet Sections

## Summary

Displays wallet balances and financial overview.

---

## Add Funds

Redirects the user to the Deposit flow.

See:

`deposit.md`

---

## Add A Card

Allows users to add a new credit or debit card.

See:

`add-card.md`

---

## Saved Cards

Displays previously saved payment cards.

Users can manage existing cards.

See:

`saved-cards.md`

---

## Cash Out

Allows users to withdraw eligible funds.

See:

`cash-out.md`

---

## Account History

Displays all wallet transactions.

Examples include:

- Deposits
- Withdrawals
- Contest Entries
- Contest Winnings
- Refunds
- Bonus Credits

See:

`account-history.md`

---

## Tickets

Displays promotional tickets available in the user's account.

See:

`tickets.md`

---

## Offers

Displays available promotional offers and deposit bonuses.

See:

`offers.md`

---

# 9. Business Rules

- Wallet is accessible only after user login.
- Deposit functionality may require completed KYC.
- Cash Out is available only for eligible balances.
- Bonus Balance may have usage restrictions.
- Available To Play is calculated using Cash Balance and eligible Bonus Balance.
- In Play balance cannot be withdrawn.
- Currently Winning updates based on live contest status.
- All wallet transactions are recorded in Account History.

---

# 10. Validation Rules

Verify:

- Cash Balance calculation.
- Bonus Balance calculation.
- Available To Play calculation.
- In Play calculation.
- Currently Winning calculation.
- Ticket count.
- Navigation to all wallet sections.
- Wallet refresh after financial transactions.

---

# 11. Positive Scenarios

- Open Wallet successfully.
- View Summary.
- Navigate to Deposit.
- Navigate to Add A Card.
- Navigate to Saved Cards.
- Navigate to Cash Out.
- Navigate to Account History.
- Navigate to Tickets.
- Navigate to Offers.
- Verify balances update after deposit.

---

# 12. Negative Scenarios

- Network unavailable.
- Wallet API failure.
- Session expired.
- Unauthorized access.
- Balance loading failure.
- Unable to retrieve wallet information.

---

# 13. Edge Cases

- Refresh Wallet during balance update.
- Multiple Wallet open requests.
- Session timeout while Wallet is open.
- Simultaneous balance updates.
- Slow API response.
- Empty transaction history.
- Zero balance account.

---

# 14. Error Messages

| Scenario | Expected Result |
|----------|-----------------|
| Network Failure | Unable to load Wallet |
| Session Expired | Please login again |
| Server Error | Something went wrong |
| Balance Unavailable | Unable to retrieve wallet information |

Use production messages whenever possible.

---

# 15. Platform Differences

| Feature | Web | Android | iOS |
|----------|-----|----------|-----|
| Wallet Summary | Supported | Supported | Supported |
| Add Funds | Supported | Supported | Supported |
| Add A Card | Supported | Supported | Supported |
| Saved Cards | Supported | Supported | Supported |
| Cash Out | Supported | Supported | Supported |
| Account History | Supported | Supported | Supported |
| Tickets | Supported | Supported | Supported |
| Offers | Supported | Supported | Supported |

---

# 16. Admin Configuration

Administrators can configure:

- Wallet enable/disable.
- Cash Balance calculation.
- Bonus calculation rules.
- Ticket allocation.
- Deposit availability.
- Cash Out eligibility.
- Offers visibility.
- Responsible Gaming limits.
- Feature flags.

---

# 17. Test Data

| Scenario | Test Data |
|----------|-----------|
| New User | Zero balance |
| Existing User | Positive balance |
| Bonus User | Bonus available |
| Ticket User | Tickets available |
| Contest User | In Play balance |
| Winning User | Currently Winning amount |

---

# 18. Automation Strategy

### UI Automation

- Wallet navigation.
- Summary validation.
- Balance verification.
- Navigation to all Wallet sections.
- Balance refresh after deposit.
- Balance refresh after contest join.

### API Automation

- Wallet API.
- Balance API.
- Ticket API.

### Regression

- Cross-browser.
- Android.
- iOS.

Recommended Frameworks:

- Playwright
- Appium

---

# 19. AI Implementation

AI should be able to:

- Generate Wallet automation.
- Validate balance calculations.
- Generate Wallet API tests.
- Generate regression scenarios.
- Review Wallet business rules.

---

# 20. Dependencies

- Authentication
- Deposit
- Add Card
- Saved Cards
- Cash Out
- Account History
- Offers
- Tickets
- Responsible Gaming

---

# 21. Security Considerations

- HTTPS communication.
- Authenticated session.
- Secure financial APIs.
- Authorization validation.
- Secure wallet balance retrieval.

---

# 22. Performance Considerations

- Wallet should load within acceptable response time.
- Balance updates should be reflected immediately after successful transactions.
- Navigation between Wallet sections should be responsive.

---

# 23. Accessibility Considerations

Verify:

- Keyboard navigation.
- Screen reader compatibility.
- Focus order.
- Color contrast.
- Readable financial information.

---

# 24. Related Modules

- Deposit
- Add Card
- Saved Cards
- Cash Out
- Account History
- Offers
- Tickets
- KYC

---

# 25. Known Issues

Document current Wallet-related issues.

Leave blank if none exist.

---

# 26. Future Enhancements

Document confirmed roadmap items only.

Avoid documenting speculative enhancements.

---

# 27. Related Documentation

- flows/deposit.md
- flows/add-card.md
- flows/saved-cards.md
- flows/cash-out.md
- flows/account-history.md
- flows/tickets.md
- flows/offers.md

---

# 28. Revision History

| Version | Date | Author | Description |
|----------|------|--------|-------------|
| 1.0 | YYYY-MM-DD | QA Team | Initial Version |
