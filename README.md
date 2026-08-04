# MoveitPro (moveitpro)

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
