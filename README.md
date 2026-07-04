# Aisle Planner (aisle-planner)

Aisle Planner is a cloud-based business management platform for wedding and event professionals - planners, venues, caterers, florists, and photographers - bundling lead management, proposals/contracts with e-signatures, invoicing and online payments, timelines, budgets, guest and vendor management, seating charts, event websites, and online RSVP into one system.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/aisle-planner/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/aisle-planner/refs/heads/main/apis.yml)

## API Access Model (Important)

**Aisle Planner does not publish a public, self-service developer API.** There is no developer portal, no public API reference, no OpenAPI definition, and no documented WebSocket or webhook API at the time of cataloging. This entry is intentionally a stub that documents the company and its access model honestly rather than fabricating an API surface.

How integration actually works:

- **A private key gates one integration, not a platform.** The only "API key" Aisle Planner issues is a per-account key found in Business Settings > Integrations, and its sole documented purpose is to authenticate the account inside a pre-built Zapier app.
- **Zapier is the entire third-party surface.** The Zapier integration exposes 3 documented triggers (new project, new lead, payment received) and 3 documented actions (create wedding project, create event project, create lead in CRM) - it connects Aisle Planner to 1,000+ apps like QuickBooks, Gmail, Mailchimp, WeddingWire, and The Knot, but is a managed no-code surface, not a general REST API a developer can call directly.
- **No other developer resources exist.** No `developer.aisleplanner.com` or `api.aisleplanner.com` subdomain, no public API reference, and no endpoint list, request/response schema, or base URL is disclosed anywhere on aisleplanner.com or help.aisleplanner.com.

Because no public endpoints, request/response schemas, or authentication details are documented, no `openapi/`, `collections/`, `rate-limits/`, or `finops/` artifacts are included, and no `apis` array is asserted in `apis.yml`. If Aisle Planner opens public developer API documentation in the future, this entry can be expanded with real, sourced endpoints.

## Tags

- Weddings
- Event Planning
- Business Management
- CRM
- Zapier
- Vertical SaaS
- Event Professionals

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## Pricing

Aisle Planner Pro publishes standardized, tiered monthly subscription pricing on aisleplanner.com/pricing, gated primarily by active client project count: Sales Essentials at $49.99/month (CRM/sales tools only, no project management), then $69.99/month (up to 15 projects), $109.99/month (16-25), $164.99/month (26-50), and $229.99/month (51-100); accounts needing more than 100 active projects contact sales for a custom quote. All tiers include unlimited users, custom branding, personalized onboarding, and the Zapier integration, with a minimum of two AP Connect (email/scheduling) seats included and additional seats at $10/month. Annual billing gets a 10% discount, and a 30-day free trial (credit card required) is offered. There is no separate API/developer pricing since no public developer API exists. See [Plans & Pricing](plans/aisle-planner-plans-pricing.yml).

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/aisle-planner-inc-)
- [Website](https://www.aisleplanner.com/)
- [Documentation](https://help.aisleplanner.com/)
- [Plans](plans/aisle-planner-plans-pricing.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
