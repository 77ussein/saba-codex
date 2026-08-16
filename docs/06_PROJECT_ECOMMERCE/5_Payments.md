# Payments

## Purpose

The SAB’A payment system defines how customers securely complete purchases across the ecommerce experience.

Payment is the final technical step of the transaction, but it must remain a natural continuation of the SAB’A experience.

The payment experience must be:

**Secure → Clear → Fast → Flexible → Trustworthy**

The governing principle is:

**Payment should feel effortless, while the infrastructure behind it remains rigorous.**

---

# Payment Philosophy

SAB’A should provide customers with convenient and trusted payment options without overwhelming them with unnecessary choices.

Payment methods should be selected according to:

- Customer preference
- Market
- Device
- Order value
- Eligibility
- Security
- Commercial viability

The system must always prioritise reliability and customer trust.

---

# Supported Payment Methods

The initial payment ecosystem should support relevant methods including:

- Credit cards
- Debit cards
- Apple Pay
- Samsung Pay
- Tabby
- Tamara
- Other approved local payment methods where appropriate

The payment system should remain extensible so additional methods can be introduced without restructuring the entire ecommerce architecture.

---

# Card Payments

Card payments should support appropriate major card networks available in the target market.

The experience should clearly communicate:

- Accepted card types
- Required information
- Payment status
- Success or failure

Sensitive payment information should be handled through secure payment infrastructure.

---

# Apple Pay

Apple Pay should provide a fast and familiar payment experience on supported devices and browsers.

Where available, the customer should be able to complete payment without unnecessary manual entry.

Apple Pay must remain integrated with the normal order process.

A successful Apple Pay transaction must create the same reliable order record as any other approved payment method.

---

# Samsung Pay

Samsung Pay should be supported where technically and commercially available.

The experience should follow the same principles as other digital wallets:

- Fast
- Secure
- Clear
- Consistent

The payment method must remain connected to the central ecommerce order system.

---

# Tabby

Tabby should be supported as a payment option where available and eligible.

The customer should clearly understand when choosing Tabby that the payment is being processed through a third-party payment service.

The checkout should communicate any relevant information provided by Tabby without creating unnecessary complexity.

SAB’A must not make unsupported claims regarding eligibility, approval, instalment terms, or fees.

Those details must come from the verified payment provider information available at the time of checkout.

---

# Tamara

Tamara should be supported as a payment option where available and eligible.

The customer should clearly understand the payment arrangement presented by Tamara before completing the transaction.

SAB’A must not invent or independently guarantee:

- Approval
- Instalment eligibility
- Payment schedules
- Fees
- Limits

The verified Tamara payment information presented during checkout remains authoritative.

---

# Buy Now, Pay Later

Services such as Tabby and Tamara may provide customers with flexible payment options.

However, SAB’A should present these options responsibly.

The brand should never use instalment services as aggressive sales pressure.

The customer's decision should remain informed and voluntary.

---

# Payment Method Availability

Not every payment method must appear for every customer.

Availability may depend on:

- Country
- Currency
- Device
- Browser
- Order value
- Product eligibility
- Customer eligibility
- Payment provider availability

The checkout should only display payment methods that are currently usable.

---

# Payment Method Presentation

Payment options should be presented clearly and calmly.

Each method should communicate enough information for the customer to understand what they are selecting.

Avoid unnecessary technical explanations.

The interface should prioritise:

**Recognition → Understanding → Selection**

---

# Payment Selection

The customer should be able to select their preferred payment method before final order submission.

The selected method should be clearly identifiable.

If changing the payment method affects the total or available options, the checkout should update accordingly.

---

# Payment Security

Payment security is non-negotiable.

The ecommerce infrastructure should use appropriate security measures including:

- Secure payment processing
- Encryption
- Authentication
- Fraud prevention
- Secure sessions
- Appropriate payment verification

SAB’A should minimise the storage and exposure of sensitive payment information.

---

# Payment Provider

Payment processing may rely on approved third-party payment providers.

The provider must integrate reliably with:

- Orders
- Checkout
- Customer account
- Refunds
- Customer care
- Transactional communication

The payment provider should never become a separate source of truth for the customer's overall order experience.

---

# Payment Authorisation

An order should only be considered successfully paid when the ecommerce system receives verified confirmation from the payment infrastructure.

The system must not rely solely on the customer's browser state or interface message.

---

# Payment Confirmation

After successful payment, the customer should receive immediate confirmation.

The system should communicate:

- Payment success
- Order number
- Amount paid
- Payment method
- Order status
- Next step

---

# Payment Failure

If a payment fails, the customer must receive a clear and useful message.

The system should explain where possible:

- Payment was unsuccessful
- Whether the order was created
- Whether any amount was charged
- What action to take next

Technical error codes should not be exposed unnecessarily.

---

# Failed Payment Recovery

Where possible, customers should be able to retry payment without rebuilding the entire order.

The system should preserve relevant:

- Cart contents
- Customer information
- Delivery information

Sensitive payment information must not be retained unnecessarily.

---

# Duplicate Payments

The system must protect against duplicate transactions.

This is particularly important when:

- Customers refresh the page
- Payment processing takes longer than expected
- A customer taps the payment button multiple times
- A payment provider response is delayed

The system should use appropriate transaction and order controls to prevent duplicate orders or charges.

---

# Payment Pending

Some payment methods may require additional processing time.

When a payment is pending, the customer should be told clearly:

- That the payment is still being processed
- Whether the order is created
- What they should do next
- When they can expect an update where applicable

The system must not incorrectly mark a pending payment as successful.

---

# Payment Reversal

If a payment is authorised but later reversed or fails to settle, the ecommerce system must reconcile the payment state with the order state.

Customer communication should remain accurate.

---

# Refunds

Refunds must be linked to the original transaction wherever possible.

The system should support appropriate refund states such as:

- Refund requested
- Refund processing
- Refund completed
- Refund failed

Customers should receive accurate communication about refund status.

---

# Partial Refunds

Where business rules permit, partial refunds should be supported.

The system should clearly identify:

- Refunded amount
- Remaining order value
- Products affected
- Refund status

---

# Refund Method

Refunds should normally return through the appropriate original payment method where supported.

The customer should not be given misleading expectations about refund timing.

Actual processing time may depend on the payment provider and financial institution.

---

# Payment and Returns

Returns and payment refunds must remain connected.

When a return is approved, the system should correctly determine:

- Amount eligible for refund
- Original payment method
- Applicable deductions
- Refund status

Detailed return policies are defined in:

**7_Returns and Exchanges.md**

---

# Payment and Customer Account

The customer's account should reflect relevant payment information without exposing sensitive financial data.

It may display:

- Payment method type
- Last four digits where appropriate
- Payment status
- Amount
- Refund status

Full card numbers and sensitive credentials must never be exposed.

---

# Payment and Customer Care

Customer care should be able to understand the payment state of an order.

Relevant information may include:

- Payment method
- Payment status
- Transaction reference
- Amount
- Refund status
- Failure status

Sensitive information must remain protected.

---

# Payment and AI

SAB’A AI may assist customers with general payment questions.

It may explain:

- Available payment methods
- General payment steps
- General refund status
- Where to find payment information

AI must never:

- Request full card details
- Request passwords
- Invent payment status
- Guarantee approval from Tabby or Tamara
- Guarantee a refund before confirmation
- Claim payment succeeded without verified system information

---

# Payment and Email

Transactional emails may communicate:

- Payment confirmation
- Payment failure
- Refund initiation
- Refund completion

The amount and status shown must match the ecommerce system.

---

# Payment and WhatsApp

Where WhatsApp support is enabled, customers may ask about:

- Payment status
- Failed payment
- Refund status
- General payment methods

WhatsApp communication must remain consistent with the central order and payment system.

Customers should never be asked to send sensitive card information through WhatsApp.

---

# Payment Receipts

After successful purchase, the customer should receive an appropriate receipt or transaction record.

The receipt should contain accurate information such as:

- Order number
- Date
- Products
- Amount
- Taxes where applicable
- Discounts where applicable
- Final amount
- Payment status

The receipt should remain easy to access through email and, where applicable, the customer account.

---

# Payment and Digital Wallets

The payment architecture should be capable of supporting future wallet-based experiences.

Potential future integrations may include:

- Apple Wallet
- Google Wallet
- Samsung Wallet

These may support loyalty or customer identification rather than replacing the underlying payment infrastructure.

---

# Payment and Loyalty

A successful purchase should update the customer's loyalty relationship where applicable.

The system may calculate:

- Points earned
- Rewards unlocked
- Membership progress

Loyalty calculations must be based on the final verified transaction.

---

# Payment and Promotions

The payment system must correctly reflect:

- Base price
- Coupon
- Promotional discount
- Loyalty benefit
- Shipping
- Taxes
- Final total

No payment provider should unexpectedly change the customer's confirmed ecommerce total.

---

# Payment Security and Fraud

The system should use appropriate fraud prevention mechanisms.

These may include:

- Transaction monitoring
- Risk assessment
- Authentication
- Velocity controls
- Suspicious transaction review

Fraud prevention should protect both SAB’A and customers while minimising unnecessary false declines.

---

# Payment Data

Payment data must be handled according to applicable privacy and security requirements.

SAB’A should minimise the amount of sensitive financial information stored within its own systems.

Where possible, sensitive payment credentials should remain with specialised payment providers.

---

# Payment Reconciliation

Every successful transaction should be reconcilable between:

**Customer → Ecommerce Order → Payment Provider → Financial Records**

The system should support accurate reconciliation of:

- Payments
- Refunds
- Partial refunds
- Failed transactions
- Reversals
- Fees where applicable

---

# Payment Monitoring

The business should monitor payment performance.

Important indicators may include:

- Payment success rate
- Payment failure rate
- Decline rate
- Refund rate
- Duplicate transaction rate
- Provider errors
- Payment-method performance

Unexpected changes should trigger investigation.

---

# Payment Provider Failure

If a payment provider becomes unavailable, the system should handle the situation gracefully.

Where possible:

- Inform the customer clearly
- Offer an alternative payment method
- Prevent duplicate orders
- Preserve the customer's cart
- Record the incident

The website should never expose unnecessary technical details.

---

# Payment Scalability

The payment architecture should allow SAB’A to expand into:

- New markets
- New currencies
- New payment providers
- New digital wallets
- New local payment methods

Expansion should not require rebuilding the entire ecommerce system.

---

# Payment Quality Audit

Before launching or changing a payment method, verify:

1. **Does the payment method work correctly?**
2. **Is it available in the intended market?**
3. **Is the currency supported?**
4. **Is the payment securely processed?**
5. **Is successful payment correctly linked to the order?**
6. **Are failed payments handled correctly?**
7. **Are duplicate charges prevented?**
8. **Are refunds supported?**
9. **Does customer care receive the correct payment status?**
10. **Do email and WhatsApp communications remain accurate?**
11. **Does loyalty update correctly after payment?**
12. **Does the experience work on mobile?**
13. **Does the payment method maintain SAB’A's standard of trust and refinement?**

---

# What Payments Must Never Become

The payment experience must never become:

- Confusing
- Aggressive
- Technically overwhelming
- Unsafe
- Unclear about the final amount
- Dependent on unsupported promises
- A source of contradictory order information

Customers should never have to wonder:

**"Did my payment go through?"**

---

# Core Standard

The ideal SAB’A payment experience is:

**Fast enough to disappear.  
Secure enough to trust.  
Flexible enough to accommodate customers.  
Reliable enough to support the house.**

---

# Core Statement

Payment is where the commercial decision becomes a confirmed transaction.

SAB’A must make that moment feel:

**Secure. Clear. Calm. Final.**

The system should support cards, digital wallets, **Tabby**, **Tamara**, and future payment methods without allowing the payment infrastructure to dominate the customer experience.

**The customer should remember what they bought and how SAB’A made them feel — not the payment technology behind the transaction.**

---

**SAB’A Codex**  
**Document:** 5_Payments  
**Version:** 1.0  
**Status:** Draft  
**Owner:** SAB’A  
**Last Updated:** 16 August 2026