# Ecommerce Architecture

## Purpose

The SAB’A ecommerce system defines how the commercial side of the house operates digitally.

It transforms the visitor's relationship with SAB’A from:

**Discovery → Consideration → Selection → Purchase → Delivery → Ownership → Return**

without breaking the emotional and premium character established by the wider website.

Ecommerce is therefore not a separate layer placed on top of the brand experience.

It is the commercial infrastructure that allows the experience to continue into ownership.

---

# Ecommerce Philosophy

SAB’A is a luxury house.

Its ecommerce system must therefore prioritise:

- Clarity
- Trust
- Ease
- Precision
- Service
- Restraint
- Consistency

The customer should never feel pressured into purchasing.

The system should make purchasing feel like the natural next step after desire has been established.

The governing principle is:

**Commerce should support the experience, not replace it.**

---

# Commercial Journey

The core ecommerce journey is:

**Discovery → Product → Selection → Bag → Checkout → Payment → Fulfilment → Delivery → Ownership**

Each stage must connect naturally to the next.

No stage should feel like it belongs to a different system.

---

# Ecommerce Architecture Layers

The ecommerce system is organised into the following layers:

### 1. Product Catalogue

Defines what SAB’A sells and how products are organised.

### 2. Pricing

Defines how prices, promotions, discounts, and customer benefits are managed.

### 3. Shopping Bag

Allows customers to review and manage selected products.

### 4. Checkout

Transforms product selection into a completed order.

### 5. Payments

Processes transactions securely and clearly.

### 6. Shipping

Manages fulfilment, delivery options, tracking, and communication.

### 7. Returns and Exchanges

Defines the post-purchase resolution experience.

### 8. Customer Relationship

Connects orders with the customer's account, loyalty, communication, and service history.

---

# Product Catalogue

The product catalogue is the commercial foundation of SAB’A.

Every product must have a structured representation containing relevant information such as:

- Product name
- Product identifier
- Category
- Collection
- Description
- Images
- Video where applicable
- Price
- Variants
- Size
- Availability
- Inventory status
- Product details
- Ingredients or materials where applicable
- Shipping information
- Return eligibility

The catalogue must remain accurate across all customer-facing systems.

Detailed catalogue principles are defined in:

**2_Product Catalog.md**

---

# Product Relationships

Products should not exist as isolated database entries.

They should maintain meaningful relationships with:

- Collections
- Categories
- Related creations
- Complementary products
- Customer preferences
- Loyalty benefits

This allows the ecommerce system to support discovery as well as transactions.

---

# Inventory

Inventory must be represented accurately.

The system should distinguish between:

- Available
- Low stock
- Out of stock
- Coming soon
- Pre-order where applicable

Inventory messaging must be truthful.

Artificial scarcity must not be created to manipulate customers.

---

# Product Availability

Availability should remain consistent across:

- Website
- Customer account
- Checkout
- Customer care
- Email
- WhatsApp where relevant

A customer should not be told that a product is available in one channel and unavailable in another without a legitimate reason.

---

# Pricing Architecture

Pricing must be structured and controlled.

The system should support:

- Standard pricing
- Promotional pricing
- Campaign pricing
- Customer rewards
- Coupons
- Gift cards where applicable
- Loyalty benefits

Pricing rules must remain transparent to the customer.

Detailed pricing principles are defined in:

**3_Pricing.md**

---

# Luxury and Pricing

Luxury does not mean hiding price.

Price should be:

- Visible
- Accurate
- Consistent
- Easy to understand

Promotional mechanics should be controlled carefully.

SAB’A should not train customers to wait for discounts.

The value of the product must primarily come from:

**Creation + Craft + Story + Experience + Service**

rather than price reduction.

---

# Shopping Bag

The shopping bag is the bridge between desire and transaction.

It should allow customers to:

- Review products
- Change quantities where applicable
- Remove products
- Review price
- Apply eligible coupons
- Understand shipping implications
- Continue shopping
- Proceed to checkout

The bag should remain simple.

It should not become another promotional environment.

---

# Checkout Architecture

Checkout should reduce uncertainty.

The customer should be able to understand:

- What they selected
- What they are paying
- Where the order is going
- How it will be delivered
- Which payment method is being used
- What happens after payment

The checkout journey should be focused and predictable.

Detailed principles are defined in:

**4_Checkout.md**

---

# Checkout Continuity

The checkout environment may reduce general website navigation to maintain focus.

However, it must still feel like SAB’A.

The customer should not feel as though they have suddenly entered an unrelated payment platform.

---

# Customer Information

The ecommerce system may collect information required for:

- Account creation
- Checkout
- Delivery
- Payment
- Order communication
- Customer service
- Loyalty

Only necessary information should be requested.

The customer should not be forced to provide unnecessary information simply because the system can collect it.

---

# Guest Checkout

Guest checkout may be supported where appropriate.

The objective is to avoid unnecessary friction while still allowing customers to create or connect an account.

After purchase, the customer may be invited to create an account to access:

- Order history
- Tracking
- Wishlist
- Loyalty
- Rewards
- Preferences

The invitation should feel useful rather than forced.

---

# Customer Account Integration

The ecommerce system should connect naturally to the SAB’A customer account.

Customers should be able to access:

- Orders
- Order details
- Tracking
- Purchase history
- Wishlist
- Loyalty points
- Rewards
- Coupons
- Communication preferences
- Customer care

The account becomes the long-term relationship layer between the customer and the house.

---

# Loyalty Integration

Purchases may contribute to the customer's loyalty relationship.

The system may support:

- Points accumulation
- Reward eligibility
- Product rewards
- Exclusive access
- Selected offers
- Membership benefits

The loyalty system must remain connected to real customer activity.

It should not operate as an isolated points counter.

---

# Coupons and Promotions

Coupons must be validated by the ecommerce system before being applied.

The system should verify:

- Eligibility
- Expiration
- Product restrictions
- Minimum spend where applicable
- Customer restrictions
- Usage limits
- Campaign conditions

The customer should receive a clear explanation when a coupon is invalid.

---

# Competitions and Promotional Campaigns

SAB’A may run periodic campaigns through channels such as X, Instagram, TikTok, email, or the website.

These may include:

- Promotional codes
- Product rewards
- Discovery sets
- Gift cards
- Exclusive access

Campaign mechanics must connect cleanly to ecommerce without compromising normal purchasing.

---

# Payments

Payment infrastructure must be secure, reliable, and easy to understand.

The system may support relevant payment methods appropriate to the target markets.

Potential methods may include:

- Card payments
- Digital wallets
- Local payment methods
- Other approved payment solutions

Detailed payment principles are defined in:

**5_Payments.md**

---

# Payment Failure

Payment failures must be handled clearly.

The customer should understand:

- That the payment did not complete
- Whether the order was created
- Whether the amount was charged
- What action to take next

The system should prevent duplicate orders and unnecessary repeated charges.

---

# Order Creation

An order should only be considered confirmed when the ecommerce system has successfully completed the required transaction and order creation process.

The customer should receive confirmation immediately after successful completion.

---

# Order Confirmation

After purchase, the customer should receive a clear confirmation.

The confirmation should communicate:

- Order number
- Purchased products
- Quantity
- Total
- Delivery information
- Payment status
- Expected next step
- Customer care access

---

# Transactional Email

Transactional email forms part of the ecommerce infrastructure.

It may include:

- Order confirmation
- Receipt
- Payment confirmation
- Shipping notification
- Delivery notification
- Return confirmation
- Refund confirmation

These messages should remain functional while maintaining SAB’A's identity.

---

# Shipping Architecture

Shipping must be integrated with ecommerce from the beginning.

The system should communicate:

- Delivery options
- Delivery costs
- Estimated delivery time
- Delivery location
- Tracking
- Order status

Detailed shipping principles are defined in:

**6_Shipping.md**

---

# Delivery Experience

Delivery is part of the SAB’A experience.

The digital experience should prepare the customer for the physical arrival of the product.

The transition should feel like:

**Digital Discovery → Purchase → Anticipation → Arrival → Ownership**

The order should not disappear from the customer's experience after payment.

---

# Order Tracking

Customers should be able to understand where their order is.

Tracking may be available through:

- Customer account
- Email
- WhatsApp where appropriate
- Shipping provider integration

The information should remain clear and current.

---

# Returns and Exchanges

Returns and exchanges are part of the ecommerce architecture rather than an afterthought.

The process should be:

- Clear
- Accessible
- Fair
- Structured
- Easy to understand

The customer should know:

- Eligibility
- Time limits
- Process
- Required steps
- Expected resolution

Detailed principles are defined in:

**7_Returns and Exchanges.md**

---

# Customer Care Integration

Ecommerce should connect directly to customer service.

Support may be available through:

- WhatsApp
- Customer care email
- SAB’A AI
- Human support

Customer care should have sufficient order context to resolve issues efficiently where appropriate.

---

# WhatsApp Integration

WhatsApp may support ecommerce-related communication such as:

- Order guidance
- Delivery questions
- Customer support
- Product questions
- General assistance

It should not become a replacement for the complete account and order system.

The website and account remain the central source of truth.

---

# AI Integration

SAB’A AI may support the ecommerce experience by helping customers:

- Discover products
- Understand products
- Find relevant information
- Navigate common questions
- Understand order status
- Reach customer care

AI should never invent:

- Prices
- Availability
- Shipping information
- Return policies
- Product claims

Commerce-related answers should come from verified system information.

---

# Customer Data

Customer data must remain consistent across the ecommerce ecosystem.

Relevant systems may include:

- Customer account
- Orders
- Loyalty
- Marketing preferences
- Customer care
- Email
- WhatsApp

Data should be handled securely and according to applicable privacy requirements.

---

# Order History

The customer's account should preserve meaningful purchase history.

It may include:

- Order number
- Date
- Products
- Amount
- Status
- Delivery
- Returns
- Refunds

Order history should help customers manage their relationship with SAB’A.

---

# Post-Purchase Experience

The ecommerce relationship does not end at payment.

The system should support:

**Confirmation → Fulfilment → Delivery → Ownership → Care → Loyalty → Return**

The customer should continue to receive useful information without being overwhelmed.

---

# Cross-Channel Commerce

The ecommerce architecture must support customers arriving from:

- Website
- Instagram
- TikTok
- X
- Email
- WhatsApp
- Campaigns
- Direct links

A product discovered on social media should lead to a coherent product experience.

A campaign code received by email should behave predictably.

A customer asking about an order through WhatsApp should receive information consistent with their account.

---

# Scalability

The architecture must support future growth.

It should be capable of accommodating:

- More products
- More collections
- More customers
- Additional markets
- Additional currencies
- Additional payment methods
- Additional shipping options
- Loyalty expansion
- Digital wallet integration
- New customer service capabilities
- AI development

Growth must not require rebuilding the entire commerce foundation.

---

# Technical Principle

Technology must support the commercial architecture.

The system should prioritise:

- Reliability
- Security
- Performance
- Scalability
- Maintainability
- Accurate data
- Integration

Technology decisions must support the customer experience.

---

# Ecommerce Quality Standard

Before launching a commerce experience, verify:

1. **Is the product information accurate?**
2. **Is the price accurate?**
3. **Is availability accurate?**
4. **Can the customer purchase without unnecessary friction?**
5. **Are payment methods reliable?**
6. **Are shipping expectations clear?**
7. **Can the customer track the order?**
8. **Can the customer access their order history?**
9. **Are returns and exchanges understandable?**
10. **Can customer care access the right context?**
11. **Are loyalty and rewards integrated correctly?**
12. **Do coupons behave predictably?**
13. **Do email and WhatsApp communications remain consistent?**
14. **Does the entire journey feel like SAB’A?**

---

# What Ecommerce Must Never Become

SAB’A ecommerce must never feel like:

- A discount engine
- A complicated checkout system
- A generic marketplace
- A collection of disconnected tools
- A technical payment interface
- An aggressive sales funnel

Commerce must remain calm.

Clear.

Trustworthy.

Premium.

---

# Core Standard

The ecommerce system should make buying easy without making the brand feel ordinary.

It should remove friction without removing emotion.

It should provide information without overwhelming the customer.

It should support transactions without allowing transactions to define the entire relationship.

The ideal experience is:

**Easy to Buy. Difficult to Forget.**

---

# Core Statement

SAB’A ecommerce is the commercial infrastructure of the house.

It connects:

**Product → Price → Bag → Checkout → Payment → Shipping → Delivery → Ownership → Loyalty**

while remaining connected to:

**Website → Account → Email → WhatsApp → AI → Customer Care → Social**

The customer should experience one continuous relationship.

**The transaction is not the end of the experience.**

**It is the point where the digital relationship becomes physical.**

---

**SAB’A Codex**  
**Document:** 1_Ecommerce Architecture  
**Version:** 1.0  
**Status:** Draft  
**Owner:** SAB’A  
**Last Updated:** 16 August 2026