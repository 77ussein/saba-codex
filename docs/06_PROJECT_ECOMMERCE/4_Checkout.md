# Checkout

## Purpose

The SAB’A checkout is the final commercial stage of the digital experience.

It transforms:

**Desire → Decision → Transaction → Confirmation**

The checkout must remove unnecessary friction while preserving the confidence, clarity, and refinement established throughout the SAB’A experience.

It should feel:

**Calm. Clear. Secure. Effortless.**

The governing principle is:

**The easier the purchase becomes, the more invisible the system should feel.**

---

# Checkout Philosophy

Checkout is not a place for excessive storytelling, promotional pressure, or unnecessary navigation.

By the time a customer reaches checkout, the decision should already feel made.

The role of checkout is to make completion effortless.

It must provide enough information to create confidence without overwhelming the customer.

---

# Checkout Journey

The primary checkout sequence is:

**Bag → Information → Delivery → Payment → Review → Confirmation**

The exact implementation may vary depending on the payment and commerce infrastructure.

The underlying logic must remain simple.

---

# Checkout Principles

The checkout must prioritise:

- Clarity
- Speed
- Trust
- Accuracy
- Security
- Accessibility
- Error prevention
- Mobile usability

Every additional step must have a reason to exist.

---

# Checkout Entry

Before entering checkout, the customer should be able to confirm:

- Products
- Quantities
- Selected variants
- Subtotal
- Applied discounts
- Estimated shipping
- Estimated total where available

The customer should never enter checkout with uncertainty about what they are purchasing.

---

# Shopping Bag Review

The bag should function as the final review point before checkout.

Customers should be able to:

- Increase or decrease quantities where applicable
- Remove products
- Review variants
- Apply eligible coupons
- Review subtotal
- Understand shipping
- Continue shopping
- Proceed to checkout

Changes must update pricing and availability accurately.

---

# Guest Checkout

Guest checkout should be supported where commercially and technically appropriate.

Customers should not be forced to create an account before purchasing unless there is a legitimate business requirement.

After purchase, the customer may be invited to create an account.

The invitation should communicate the value of doing so, such as access to:

- Order history
- Tracking
- Loyalty
- Rewards
- Wishlist
- Preferences

---

# Customer Account Checkout

Existing customers should be able to sign in easily.

Where an account is recognised, the checkout may securely use relevant stored information such as:

- Name
- Contact information
- Saved addresses
- Eligible loyalty benefits

The customer must remain in control of their information.

---

# Contact Information

Checkout should request only information required to complete the transaction and fulfil the order.

Typical information may include:

- Name
- Email
- Phone number

Information should be labelled clearly.

---

# Email Address

The email address is important for transactional communication.

It may be used to deliver:

- Order confirmation
- Receipt
- Payment confirmation
- Shipping updates
- Delivery confirmation
- Return or refund updates

The customer should understand the purpose of transactional communication.

---

# Phone Number

A phone number may be required for:

- Delivery
- Order communication
- Customer care
- WhatsApp communication where applicable

The system should clearly distinguish required information from optional information.

---

# Delivery Address

Address entry must be simple and accurate.

The system should support appropriate address fields for the relevant market.

Customers should be able to review their address before placing the order.

Where supported, address assistance may reduce errors.

---

# Saved Addresses

Logged-in customers may use saved addresses.

They should be able to:

- Select an address
- Add an address
- Edit an address
- Remove an address where appropriate

The system must clearly identify the selected delivery address.

---

# Delivery Options

Available delivery options should be presented clearly.

Each option should communicate, where applicable:

- Service level
- Estimated delivery time
- Cost
- Relevant conditions

The customer should not need to search elsewhere for basic delivery information.

---

# Shipping Cost

Shipping costs must be visible before payment confirmation.

If free shipping applies, the customer should clearly understand the eligibility.

No unexpected shipping charge should appear at the final moment.

---

# Estimated Delivery

Estimated delivery should be presented as accurately as possible.

The system should avoid unrealistic promises.

If the delivery estimate changes after purchase, the customer should be informed through the appropriate communication channel.

---

# Payment

Payment should feel like a natural continuation of checkout.

The system may support relevant methods such as:

- Credit and debit cards
- Digital wallets
- Local payment methods
- Other approved payment solutions

Payment methods should be presented according to the customer's market and eligibility.

Detailed payment infrastructure is defined in:

**5_Payments.md**

---

# Payment Security

Payment information must be handled using appropriate secure payment infrastructure.

SAB’A should minimise unnecessary exposure of sensitive payment information.

Customers should receive clear indicators that the payment process is secure without cluttering the interface with technical information.

---

# Digital Wallets

Where supported, digital wallets may provide faster checkout.

Potential examples include:

- Apple Pay
- Google Pay
- Samsung Pay

Wallet availability should depend on:

- Device
- Browser
- Market
- Payment infrastructure

The wallet experience should remain consistent with the overall checkout.

---

# Payment Failure

If payment fails, the customer must receive a clear explanation.

The system should communicate:

- That the payment did not complete
- Whether the order was created
- Whether the customer was charged
- What to do next

The system must prevent accidental duplicate orders or repeated charges wherever possible.

---

# Coupon Application

Customers should be able to apply eligible coupons before completing payment.

The checkout must clearly display:

- Coupon applied
- Discount amount
- Updated total

If a coupon cannot be applied, the customer should understand why.

Detailed coupon rules are defined in:

**3_Pricing.md**

---

# Loyalty Benefits

Where applicable, customers should be able to use eligible loyalty benefits during checkout.

This may include:

- Points
- Rewards
- Coupons
- Complimentary products
- Member benefits

The system must clearly show the effect of any benefit on the final total.

---

# Order Summary

The order summary must remain visible and understandable.

It should communicate:

- Products
- Quantities
- Variants
- Subtotal
- Discounts
- Shipping
- Taxes where applicable
- Final total

The final amount should be unmistakable.

---

# Tax

Where applicable, taxes must be handled according to the requirements of the relevant market.

The customer should understand whether displayed prices are:

- Tax-inclusive
- Tax-exclusive

The final payable amount must reflect the correct tax treatment.

---

# Currency

The checkout currency must remain consistent with the customer's shopping journey.

A currency should not unexpectedly change at checkout.

If currency conversion or market selection is relevant, it must be communicated clearly.

---

# Order Review

Before final submission, the customer should have an opportunity to review:

- Products
- Quantity
- Delivery address
- Delivery method
- Payment method
- Discounts
- Final total

The final action should clearly indicate that the customer is placing an order.

---

# Primary Checkout Action

The final purchase action must be unmistakable.

Its language should clearly communicate completion, such as:

**Place Order**

or another approved SAB’A term.

Avoid vague actions that make the customer uncertain about what happens after clicking.

---

# Double Submission Protection

The system must protect against accidental duplicate submissions.

This may include:

- Temporary button state
- Processing indicator
- Transaction locking
- Duplicate order detection

The customer should receive clear feedback while the order is being processed.

---

# Order Confirmation

After a successful transaction, the customer should immediately receive a confirmation experience.

The confirmation should communicate:

- Order number
- Products
- Quantity
- Total
- Payment status
- Delivery information
- Expected next step
- Customer care access

---

# Confirmation Page

The confirmation page should feel like the beginning of anticipation, not simply a technical receipt.

It may provide:

- Order summary
- Delivery estimate
- Tracking access when available
- Account creation invitation
- Loyalty information
- Relevant next steps

The page should remain calm and focused.

---

# Transactional Email

The customer should receive an order confirmation email.

It should contain accurate information about:

- Order
- Products
- Quantity
- Total
- Payment
- Delivery
- Customer support

The email should use the same SAB’A identity while remaining primarily functional.

---

# Post-Purchase Communication

The ecommerce relationship continues after checkout.

Relevant communications may include:

**Order Confirmation → Payment Confirmation → Shipping Update → Delivery Confirmation**

Additional messages may be sent when required for:

- Delays
- Changes
- Returns
- Refunds
- Customer care

---

# WhatsApp Continuity

Where WhatsApp communication is enabled, the customer may receive or request relevant order assistance through WhatsApp.

The information must remain consistent with:

- Website
- Customer account
- Email
- Order system

WhatsApp must never become a separate source of conflicting order information.

---

# Customer Care

Customers must have an accessible path to support during checkout.

Support may include:

- SAB’A AI
- Customer care email
- WhatsApp
- Human support

The appropriate channel should depend on the nature of the issue.

---

# SAB’A AI During Checkout

AI may assist with:

- Product questions
- Shipping questions
- Payment guidance
- General checkout questions
- Policy explanations

AI must never:

- Invent prices
- Promise unavailable discounts
- Guarantee delivery times without verified information
- Claim a payment succeeded without confirmation
- Modify an order without authorised system capability

---

# Error Handling

Checkout errors must be clear and actionable.

The system should explain:

**What happened → Why it happened where useful → What to do next**

Examples may include:

- Missing information
- Invalid address
- Payment failure
- Expired coupon
- Product unavailable
- Session timeout

Technical system messages should never be exposed unnecessarily.

---

# Inventory Changes During Checkout

If a product becomes unavailable during checkout, the customer must be informed clearly.

The system should:

- Identify the affected product
- Explain the issue
- Prevent an invalid order
- Offer an appropriate next action

The system must not silently change the customer's order.

---

# Session Timeout

If a checkout session expires, the customer should receive a clear explanation.

Where possible, previously entered non-sensitive information should be preserved safely.

The customer should not be forced to restart unnecessarily.

---

# Accessibility

Checkout must be fully accessible.

This includes:

- Clear labels
- Keyboard support
- Screen-reader compatibility
- Appropriate contrast
- Clear focus states
- Adequate touch targets
- Understandable errors
- Logical information order

Accessibility is part of the checkout standard.

---

# Mobile Checkout

Mobile checkout must receive dedicated attention.

The experience should support:

- One-handed interaction where practical
- Appropriate keyboards
- Large enough touch targets
- Minimal unnecessary typing
- Fast payment
- Clear order review

Mobile checkout must never feel like a desktop form squeezed onto a phone.

---

# Checkout Performance

Checkout must be lightweight and responsive.

Performance priorities include:

- Fast page transitions
- Fast payment interface
- Minimal unnecessary scripts
- Stable rendering
- Reliable form submission

A slow checkout damages trust disproportionately.

---

# Privacy

Checkout must handle customer information responsibly.

The system should collect only what is necessary.

Customers should understand relevant:

- Privacy practices
- Communication preferences
- Data usage

Marketing consent should not be confused with transactional requirements.

---

# Security and Fraud Protection

The ecommerce system should implement appropriate security and fraud prevention measures.

These may include:

- Secure authentication
- Payment verification
- Fraud detection
- Rate limiting
- Session protection
- Secure data handling

Security measures should protect customers without creating unnecessary friction.

---

# Checkout and Loyalty

A completed purchase should update the customer's relationship with SAB’A where applicable.

After successful order completion, the system may update:

- Loyalty points
- Membership status
- Rewards
- Purchase history
- Customer account

Updates should be accurate and clearly reflected.

---

# Checkout and Customer Account

After purchase, the order should become accessible through the customer's account when an account exists.

The customer should be able to view:

- Order number
- Products
- Status
- Delivery
- Payment
- Returns
- Refunds

---

# Checkout and Analytics

Checkout analytics may measure:

- Checkout initiation
- Step progression
- Abandonment
- Payment success
- Payment failure
- Coupon usage
- Completed orders

Analytics should be used to identify friction and improve the experience.

Customer privacy must remain protected.

---

# Checkout Quality Audit

Before launch, test:

1. **Can a new customer complete checkout easily?**
2. **Can a returning customer use their account smoothly?**
3. **Does guest checkout work where enabled?**
4. **Are product details and quantities correct?**
5. **Are prices correct?**
6. **Are coupons correct?**
7. **Are loyalty benefits correct?**
8. **Are shipping options clear?**
9. **Are taxes handled correctly?**
10. **Do payment methods work?**
11. **Are payment failures handled safely?**
12. **Are duplicate orders prevented?**
13. **Does the confirmation appear immediately?**
14. **Does the confirmation email contain accurate information?**
15. **Does mobile checkout feel effortless?**
16. **Is the experience accessible?**
17. **Can customer care support the customer if something goes wrong?**
18. **Does the entire process still feel like SAB’A?**

---

# What Checkout Must Never Become

Checkout must never feel like:

- A maze
- A long registration form
- A sales funnel
- A discount trap
- A technical payment screen
- A surprise-cost experience
- A generic third-party interface

The customer should never feel punished for deciding to buy.

---

# Core Standard

The ideal SAB’A checkout is almost invisible.

The customer knows:

**What they are buying.  
What they are paying.  
Where it is going.  
How it will arrive.  
What happens next.**

Everything else should stay out of the way.

---

# Core Statement

Checkout is the moment when desire becomes commitment.

SAB’A must make that transition:

**Clear enough to trust.  
Fast enough to feel effortless.  
Secure enough to feel confident.  
Refined enough to remain worthy of the house.**

The objective is not simply to complete an order.

It is to complete the relationship's first commercial exchange without breaking the experience.

**A perfect checkout should feel like the natural final step of a decision the customer already wanted to make.**

---

**SAB’A Codex**  
**Document:** 4_Checkout  
**Version:** 1.0  
**Status:** Draft  
**Owner:** SAB’A  
**Last Updated:** 16 August 2026