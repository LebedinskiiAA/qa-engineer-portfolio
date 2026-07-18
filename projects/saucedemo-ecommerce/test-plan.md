# Test Plan — SauceDemo E-commerce

**Plan ID:** SD-TP-001  
**Version:** 1.0  
**Author:** Aleksandr Lebedinskii  
**Date:** 18 July 2026

## 1. Objective

Verify that a customer can authenticate, browse products, manage the cart and reach checkout without data loss or misleading feedback.

## 2. In scope

- Valid, invalid and locked-user authentication
- Inventory content and price display
- Product sorting
- Add/remove cart behavior and cart badge
- Checkout required-field validation
- Logout and session termination
- Basic keyboard and semantic-link observations

## 3. Out of scope

Payment processing, performance/load, third-party social links, backend security assessment and destructive testing.

## 4. Test approach

Risk-based functional testing using positive, negative, boundary, state-transition and exploratory techniques. Critical path: Login → Product → Cart → Checkout.

## 5. Entry / exit criteria

Entry: site available and public test credentials displayed.  
Exit: all P0/P1 cases executed; no open blocker; summary and defects documented.

## 6. Risks

The target is a training application and contains deliberately faulty user profiles. Findings are portfolio evidence, not claims about a commercial production system.

