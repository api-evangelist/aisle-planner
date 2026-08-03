# Aisle Planner (aisle-planner)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
