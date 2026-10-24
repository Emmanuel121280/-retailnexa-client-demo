# RetailNexa production roadmap

## Verified now
Static public marketing website only. GitHub Pages cannot run PHP, MySQL, payment webhooks or background jobs.

## Evidence and status
FEATURE_SCOPE.md records documented scope, not audited production readiness. Previously developed inventory, POS, finance, AI, subscriptions and customer modules remain unverified. Industry extensions and marketplace are future work. WhatsApp onboarding and Apple MDM are incomplete. No device control claims are validated.

## Phase 1 — authorized source audit
Obtain a sanitized PHP/MySQL source checkout and schema, without customer data or secrets. Map routes, migrations and dependencies. Check tenant isolation, ID tampering, roles, CSRF, authentication, email verification, uploads, audit logs and encrypted tokens. Preserve production unchanged; use staging fixtures.

## Phase 2 — core business reliability
Validate stock movements, selling units, returns, receipts, register balancing, completed versus outstanding profit, duplicate expense prevention, payroll and ledgers. Test tenant boundaries and concurrent updates. Define acceptance criteria with owners.

## Phase 3 — integrations
Use Paystack sandbox and signed, idempotent webhooks for payments and upgrades. Use an approved WhatsApp route such as 360dialog, with business authorization, consent, template rules, tenant-scoped credentials, retries and human handover. AI requires server-side keys, access controls, data minimization, cost limits and evaluations. No approvals are implied.

## Phase 4 — expansion
Build and pilot appointments, loyalty, industry modules and marketplace separately. Device identification is distinct from location tracking or locking. Ship controls only after supported platform enrollment, authorization and end-to-end verification.

## Phase 5 — deployment gate
Evaluate a PHP-compatible managed VPS or application host with MySQL, TLS, workers, scheduled jobs, backups and monitoring. A later VPS can reuse the existing PHP stack; compare costs before selecting. No paid service is purchased or activated. Keep credentials in environment secrets, validate restore procedures, run security and load tests, and prepare rollback. Production changes require a separately authorized release.

## Current blockers
Authorized source access, staging backend, mailbox delivery verification, provider approvals, current plan validation and real workflow tests. Historical prices are reference only.
