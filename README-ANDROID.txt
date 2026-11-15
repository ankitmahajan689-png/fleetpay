FLEETPAY V2.1 — ANDROID LOCAL STARTER

SETUP
1. Download and extract this ZIP on your Android phone.
2. Open index.html in Chrome. If local file scripts are blocked, open it in a free HTML editor/preview app.
3. Demo sign-ins:
   Administrator: admin@fleetpay.local / Admin123!
   Merchant: merchant@demo.local / Merchant123!
   Employee: employee@demo.local / Employee123!

WHAT'S INCLUDED
- Three demo roles and role-specific navigation.
- Admin merchant management.
- Employee directory.
- Demo transaction records and commission estimates.
- Terminal inventory.
- Clover vs Moneris comparison.
- Local browser storage.

LIMITATIONS
This is a prototype, not production-grade authentication or authorization. Passwords are in the HTML source, localStorage can be inspected/changed and data can be erased. Records do not sync across devices. Employee records do not create actual login accounts. All transactions are demo-only; no payments are processed and no card data is collected. Do not use for real customer or merchant records.

PROVIDER COMPARISON
Clover: Hosted Checkout redirects customers to a Clover-hosted payment page. A multi-merchant app needs each merchant to authorize the app through OAuth. Good candidate if FleetPay will supply/manage Clover terminals.
Docs: https://docs.clover.com/dev/docs/hosted-checkout-api
      https://docs.clover.com/dev/docs/use-oauth

Moneris: provides hosted tokenization and gateway APIs. Confirm its partner/platform onboarding model and hardware fit directly with Moneris.
Docs: https://developer.moneris.com/hosted-solutions/docs/setup-guide-tokenization
      https://www.moneris.com/solutions/ecommerce/moneris-api

Before choosing, get written Canadian terms from both: processing rates, monthly fees, hardware cost, residual commission schedule, contract/cancellation fees, chargebacks, support and multi-merchant API access.

BUDGET
This local prototype uses free browser storage and has no hosting/domain cost. Defer paid hosting and domain. Processing, terminals, legal/compliance and business costs are separate.

NEXT
1. Replace demo login with secure authentication and server-enforced roles.
2. Move data to a protected cloud database with row-level security and backups.
3. Implement provider OAuth, secure server-side credentials, hosted checkout and verified webhooks.
4. Review privacy, PCI DSS scope and Canadian regulatory requirements before launch.
