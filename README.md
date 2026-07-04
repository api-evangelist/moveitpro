# MoveitPro (moveitpro)

MoveitPro (MoveitPro+) is web-based moving company management software built by professional movers, covering the full operation of a moving and storage company - CRM and lead capture, estimating and quoting, a smart dispatch board with drag-and-drop scheduling and crew assignment, fleet and maintenance management, digital bills of lading and e-signatures, itemized inventory, storage and warehouse tracking, invoicing and credit-card payments, commission tracking, and AI call transcription and QA.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/moveitpro/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/moveitpro/refs/heads/main/apis.yml)

## Access Model (Honest Assessment)

MoveitPro does **not** publish a documented public developer API. There is no developer portal, no `api.moveitpro.com` host, no API reference, no OpenAPI/Swagger, and no public authentication documentation.

- MoveitPro's own pricing/comparison page advertises **"Open API & Custom Integrations"** as a differentiating feature, but this is **not self-serve or publicly documented** - it points prospects to a demo/sales conversation.
- The **only publicly documented programmatic surface** is a **Zapier integration**, which exposes four polling triggers - *Job Closed Out*, *New Client*, *New Lead*, *Saved Estimate* - and two write actions - *Create Client*, *Create Lead*.
- MoveitPro also ships native product integrations: **QuickBooks, Twilio, Mailchimp, Google Maps, Google Calendar**.

The APIs listed in `apis.yml` are **logical resources modeled from the documented Zapier integration**. MoveitPro publishes no HTTP endpoints, base URLs, or auth details, so no OpenAPI, Postman collection, plans, rate-limits, or FinOps artifacts were fabricated. See `review.yml` for the full assessment.

## Tags

- Moving Software
- Moving Company
- Logistics
- Field Service
- Dispatch
- CRM
- Vertical SaaS

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs (Modeled - not officially documented)

### MoveitPro Clients API

Client (customer) records. Modeled from the Zapier *New Client* trigger and *Create Client* action (name, contact, referral source, branch assignment).

- **Documentation:** [https://zapier.com/apps/moveitpro/integrations](https://zapier.com/apps/moveitpro/integrations)

### MoveitPro Leads API

Sales leads captured from websites, lead providers, and Zillow. Modeled from the Zapier *New Lead* trigger and *Create Lead* action (contact, move date, origin/destination, floor counts, referral source, branch ID).

- **Documentation:** [https://zapier.com/apps/moveitpro/integrations](https://zapier.com/apps/moveitpro/integrations)

### MoveitPro Jobs API

Moving jobs and their lifecycle. Modeled from the Zapier *Job Closed Out* trigger.

- **Documentation:** [https://zapier.com/apps/moveitpro/integrations](https://zapier.com/apps/moveitpro/integrations)

### MoveitPro Estimates API

Move estimates and quotes. Modeled from the Zapier *Saved Estimate* trigger; invoices are generated downstream from estimates inside the product.

- **Documentation:** [https://zapier.com/apps/moveitpro/integrations](https://zapier.com/apps/moveitpro/integrations)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/moveitpro)
- [Website](https://www.moveitpro.com/)
- [Documentation](https://www.moveitpro.com/features-list)
- [Integrations](https://zapier.com/apps/moveitpro/integrations)
- [Plans](https://www.moveitpro.com/pricing)

## Pricing

Platform subscription is per user, per month (MoveitPro does not itemize tier prices on its own demo-gated pricing page; third-party listings report roughly $99-$199/mo entry-to-small-team ranges scaling with user count). AI calling/texting features are billed via consumption-based tokens.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
