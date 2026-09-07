                         ╔══════════════════════════════════╗
                         ║          SAB’A PLATFORM          ║
                         ║   Production E-Commerce System  ║
                         ╚══════════════════════════════════╝
                                      │
                    ┌─────────────────┴─────────────────┐
                    │                                   │
                    ▼                                   ▼
             ┌───────────────┐                   ┌────────────────┐
             │  STOREFRONT   │                   │  ADMIN HOUSE   │
             │               │                   │                │
             │ Web / Next.js │                   │ Secure Admin   │
             │ Future Mobile │                   │ Operations     │
             │ iOS / Android│                   │ RBAC / 2FA     │
             └───────┬───────┘                   └───────┬────────┘
                     │                                   │
                     └─────────────────┬─────────────────┘
                                       ▼
                         ┌─────────────────────────┐
                         │   EDGE / CDN / WAF      │
                         │                         │
                         │ Cloudflare / CDN        │
                         │ DDoS Protection         │
                         │ Bot Protection          │
                         │ TLS / Security Headers  │
                         │ Edge Caching             │
                         └────────────┬────────────┘
                                      │
                                      ▼
                         ┌─────────────────────────┐
                         │   APPLICATION LAYER     │
                         │                         │
                         │ Next.js / API Layer     │
                         │ Request Validation      │
                         │ API Routing             │
                         │ Server Actions / API    │
                         │ Dependency Boundaries   │
                         └────────────┬────────────┘
                                      │
                                      ▼
                  ╔══════════════════════════════════════════╗
                  ║        DOMAIN / BUSINESS LOGIC           ║
                  ╚══════════════════════════════════════════╝
                                      │
        ┌─────────────────────────────┼─────────────────────────────┐
        │                             │                             │
        ▼                             ▼                             ▼
┌──────────────────┐        ┌──────────────────┐        ┌──────────────────┐
│      AUTH        │        │     COMMERCE     │        │     CONTENT      │
│                  │        │                  │        │                  │
│ Users            │        │ Products         │        │ CMS              │
│ Profiles         │        │ Variants         │        │ Pages            │
│ OTP              │        │ SKU              │        │ Collections      │
│ Sessions         │        │ Pricing          │        │ Categories       │
│ Permissions      │        │ Inventory        │        │ Media            │
│ Account Security │        │ Cart             │        │ SEO Content      │
└────────┬─────────┘        │ Wishlist         │        └────────┬─────────┘
         │                  │ Coupons          │                 │
         │                  │ Gift Cards       │                 │
         │                  │ Loyalty          │                 │
         │                  └────────┬─────────┘                 │
         │                           │                           │
         │                           ▼                           │
         │                  ┌──────────────────┐                 │
         │                  │      ORDERS      │                 │
         │                  │                  │                 │
         │                  │ Order Creation   │                 │
         │                  │ Order State      │                 │
         │                  │ Order Items      │                 │
         │                  │ Refunds          │                 │
         │                  │ Returns          │                 │
         │                  │ Invoices         │                 │
         │                  └────────┬─────────┘                 │
         │                           │                           │
         │              ┌────────────┴────────────┐              │
         │              ▼                         ▼              │
         │     ┌──────────────────┐      ┌──────────────────┐   │
         │     │     PAYMENTS     │      │     SHIPPING     │   │
         │     │                  │      │                  │   │
         │     │ Payment Intent   │      │ Rates            │   │
         │     │ Payment Status   │      │ Delivery         │   │
         │     │ Verification     │      │ Tracking         │   │
         │     │ Refunds          │      │ Returns          │   │
         │     │ Webhooks         │      │ Webhooks         │   │
         │     │ Idempotency      │      │ Status Updates   │   │
         │     └────────┬─────────┘      └────────┬─────────┘   │
         │              │                         │              │
         └──────────────┴──────────────┬──────────┴──────────────┘
                                       │
                                       ▼
                         ╔═════════════════════════╗
                         ║   APPLICATION SERVICES  ║
                         ║                         ║
                         ║ Use Cases               ║
                         ║ Transactions            ║
                         ║ Pricing Rules           ║
                         ║ Inventory Rules         ║
                         ║ Order Orchestration     ║
                         ║ Payment Orchestration   ║
                         ║ Shipping Orchestration  ║
                         ╚════════════╤════════════╝
                                      │
                                      ▼
                         ╔═════════════════════════╗
                         ║   INFRASTRUCTURE LAYER  ║
                         ╚════════════╤════════════╝
                                      │
       ┌──────────────────────────────┼──────────────────────────────┐
       │                              │                              │
       ▼                              ▼                              ▼
┌──────────────────┐         ┌──────────────────┐         ┌──────────────────┐
│    PostgreSQL    │         │      Redis       │         │   Search Engine  │
│                  │         │                  │         │                  │
│ Main Database    │         │ Cache            │         │ Meilisearch /    │
│ Users            │         │ Sessions*        │         │ Algolia / Other  │
│ Products         │         │ Temporary Data   │         │                  │
│ Orders           │         │ Rate Limits      │         │ Full-text Search │
│ Inventory        │         │ Performance      │         │ Autocomplete     │
│ Payments         │         │                  │         │ Faceted Filters  │
│ Audit Logs       │         │                  │         │ Arabic / English │
└────────┬─────────┘         └────────┬─────────┘         └────────┬─────────┘
         │                            │                            │
         │                            │                            │
         ▼                            ▼                            ▼
┌──────────────────┐         ┌──────────────────┐         ┌──────────────────┐
│   Read Replicas  │         │  Cache Strategy  │         │ Search Indexing  │
│                  │         │                  │         │                  │
│ Read Scaling     │         │ Cache Invalidation│        │ Product Sync     │
│ High Traffic     │         │ SWR / Revalidate │         │ Collection Sync  │
│ Future Scaling   │         │ Edge + App Cache │         │ Search Updates   │
└──────────────────┘         └──────────────────┘         └──────────────────┘
         │
         │
         └──────────────────────┬───────────────────────────────┐
                                │                               │
                                ▼                               ▼
                     ┌──────────────────┐             ┌──────────────────┐
                     │  MESSAGE QUEUE   │             │  BACKGROUND JOBS │
                     │                  │             │                  │
                     │ BullMQ / Queue   │             │ Emails           │
                     │ Event Processing │             │ Notifications    │
                     │ Async Tasks      │             │ Search Indexing  │
                     │ Retry / Backoff  │             │ Reports          │
                     │ Dead Letter      │             │ Cleanup          │
                     └────────┬─────────┘             │ Scheduled Jobs   │
                              │                       └──────────────────┘
                              ▼
                     ┌──────────────────┐
                     │ EVENT PROCESSING │
                     │                  │
                     │ Domain Events    │
                     │ Webhook Events   │
                     │ Payment Events   │
                     │ Shipping Events │
                     │ Idempotency      │
                     │ Event Logging    │
                     └────────┬─────────┘
                              │
                              ▼
                  ╔══════════════════════════════╗
                  ║      EXTERNAL SERVICES       ║
                  ╚══════════════════════════════╝
                              │
       ┌──────────────┬───────┼────────┬──────────────┬──────────────┐
       │              │       │        │              │              │
       ▼              ▼       ▼        ▼              ▼              ▼
┌────────────┐ ┌────────────┐ ┌──────┐ ┌────────────┐ ┌────────────┐ ┌────────────┐
│  PAYMENT   │ │  SMS / OTP │ │Email │ │  SHIPPING  │ │ AI / Future │ │ Analytics  │
│            │ │            │ │      │ │            │ │ Services    │ │            │
│ Mada       │ │ OTP        │ │Order │ │ Carriers   │ │ AI Search   │ │ Analytics  │
│ Apple Pay  │ │ SMS        │ │Reset │ │ Tracking   │ │ Recommend.  │ │ Conversion │
│ Visa       │ │            │ │Promo │ │ Rates      │ │ Automation  │ │ Revenue    │
│ Mastercard │ │            │ │      │ │ Returns    │ │             │ │ Events     │
└────────────┘ └────────────┘ └──────┘ └────────────┘ └────────────┘ └────────────┘
                                     
                                      │
                                      ▼
                         ┌─────────────────────────┐
                         │     FILE / MEDIA        │
                         │        STORAGE          │
                         │                         │
                         │ Object Storage          │
                         │ S3 / Cloudflare R2      │
                         │ Product Images          │
                         │ Videos                  │
                         │ Documents               │
                         │ Optimized Media         │
                         │ CDN Delivery            │
                         └─────────────────────────┘


══════════════════════════════════════════════════════════════════════════════
                         CROSS-CUTTING CONCERNS
══════════════════════════════════════════════════════════════════════════════

        ┌────────────────┬────────────────┬────────────────┬────────────────┐
        │                │                │                │                │
        ▼                ▼                ▼                ▼                ▼
┌──────────────┐ ┌──────────────┐ ┌──────────────┐ ┌──────────────┐ ┌──────────────┐
│  SECURITY    │ │   AUTH &     │ │   LOGGING    │ │  MONITORING  │ │   RELIABILITY│
│              │ │ AUTHORIZATION│ │   & AUDIT    │ │              │ │              │
│ WAF          │ │              │ │              │ │ Sentry       │ │ Health Checks│
│ DDoS         │ │ RBAC         │ │ Audit Logs   │ │ Metrics      │ │ Auto Restart │
│ Rate Limit   │ │ Sessions     │ │ Security     │ │ Alerts       │ │ Retry        │
│ Bot Protect. │ │ Admin Access │ │ Events       │ │ Uptime       │ │ Circuit Break│
│ CSRF / XSS   │ │ 2FA-ready    │ │ Admin Actions│ │ API Health   │ │ Graceful Fail│
│ SSRF         │ │ Permissions  │ │ Webhooks     │ │ DB Health    │ │ Rollback     │
└──────────────┘ └──────────────┘ └──────────────┘ └──────────────┘ └──────────────┘


══════════════════════════════════════════════════════════════════════════════
                           DATA & PLATFORM SAFETY
══════════════════════════════════════════════════════════════════════════════

                     ┌─────────────────────────┐
                     │      DATA SAFETY        │
                     └────────────┬────────────┘
                                  │
          ┌───────────────────────┼───────────────────────┐
          │                       │                       │
          ▼                       ▼                       ▼
┌──────────────────┐    ┌──────────────────┐    ┌──────────────────┐
│     BACKUPS      │    │ DISASTER RECOVERY│    │    DATABASE      │
│                  │    │                  │    │    PROTECTION    │
│ Automatic        │    │ Recovery Plan    │    │ Transactions     │
│ Scheduled        │    │ Restore Testing  │    │ Constraints      │
│ Retention        │    │ Failover Strategy│    │ Connection Pool  │
│ Point-in-Time    │    │ Recovery Targets │    │ Query Protection │
└──────────────────┘    └──────────────────┘    └──────────────────┘


══════════════════════════════════════════════════════════════════════════════
                         OBSERVABILITY & OPERATIONS
══════════════════════════════════════════════════════════════════════════════

                            SAB’A SYSTEM
                                 │
             ┌───────────────────┼───────────────────┐
             ▼                   ▼                   ▼
        APPLICATION           DATABASE           INFRASTRUCTURE
             │                   │                   │
             ▼                   ▼                   ▼
           Logs              Queries              Metrics
             │                   │                   │
             └───────────────────┼───────────────────┘
                                 ▼
                         Monitoring / Alerts
                                 │
                                 ▼
                         Detect → Alert
                                 │
                                 ▼
                       Investigate → Fix
                                 │
                                 ▼
                         Test → Deploy
                                 │
                                 ▼
                           Verify


══════════════════════════════════════════════════════════════════════════════
                              DEPLOYMENT FLOW
══════════════════════════════════════════════════════════════════════════════

                             Git Repository
                                  │
                                  ▼
                           Development
                                  │
                                  ▼
                            Automated CI
                                  │
                ┌─────────────────┼─────────────────┐
                ▼                 ▼                 ▼
             Lint             Typecheck          Tests
                │                 │                 │
                └─────────────────┼─────────────────┘
                                  ▼
                             Build / Preview
                                  │
                                  ▼
                              Staging
                                  │
                    ┌─────────────┼─────────────┐
                    ▼             ▼             ▼
                  QA         Security       Performance
                    │             │             │
                    └─────────────┼─────────────┘
                                  ▼
                         Production Deploy
                                  │
                                  ▼
                         Health Verification
                                  │
                                  ▼
                         Monitoring / Alerts
                                  │
                                  ▼
                       Rollback if Required


══════════════════════════════════════════════════════════════════════════════
                         FUTURE PLATFORM SCALE
══════════════════════════════════════════════════════════════════════════════

                              SAB’A API
                                 │
             ┌───────────────────┼───────────────────┐
             │                   │                   │
             ▼                   ▼                   ▼
        Web Store            iPhone App          Android App
             │                   │                   │
             └───────────────────┼───────────────────┘
                                 ▼
                         Shared Backend / API
                                 │
                                 ▼
                          Shared Business Logic
                                 │
                                 ▼
                          Shared Data Layer


══════════════════════════════════════════════════════════════════════════════
                            BUILD STRATEGY
══════════════════════════════════════════════════════════════════════════════

PHASE 0
Inspect Existing Project
        ↓
PHASE 1
Architecture Blueprint
        ↓
PHASE 2
Foundation
        ↓
PHASE 3
Commerce Core
        ↓
PHASE 4
Admin House
        ↓
PHASE 5
Storefront
        ↓
PHASE 6
Payments / Shipping / OTP / Integrations
        ↓
PHASE 7
Security / Performance / SEO / Analytics
        ↓
PHASE 8
Testing / Load / Stress / Failure Recovery
        ↓
PHASE 9
Staging
        ↓
PHASE 10
Production Launch
        ↓
PHASE 11
Continuous Monitoring / Optimization / Scaling