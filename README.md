<a href="https://circularappliances.com">
  <img src="https://raw.githubusercontent.com/HaydenAlberighi/HaydenAlberighi/main/assets/profile-banner.png" width="100%" alt="Hayden Della Casa Alberighi — Co-Founder & Director of Operations, Circular Appliance Co." />
</a>

<div align="center">

[circularappliances.com](https://circularappliances.com) · [Partnership prospectus](https://circularappliances.com/prospectus) · [hayden@circularappliances.com.au](mailto:hayden@circularappliances.com.au)

</div>

---

## What I do

I'm a co-founder and the **Director of Operations** at [Circular Appliance Co.](https://circularappliances.com), a Brisbane social enterprise. I own the workshop and everything that moves through it — collection, triage, repair, electrical safety certification, quality control and delivery. I also designed and built the platform it runs on.

| | |
| :--- | :--- |
| **Operations** | Workshop and WHS, logistics, inventory, parts and salvage. Everything between a machine arriving and a warrantied appliance leaving the floor. |
| **Safety & quality** | AS/NZS 3760 test-and-tag with licensed supervisor sign-off. I hold final release authority — the warranty depends on that standard, not on a promise. |
| **Engineering** | The public website, operations dashboard, integration hub and API. Architecture through deployment; I wrote it. |
| **Training** | The workshop doubles as a paid, supervised pathway into the trades. I designed and run that side of it too. |

---

## The business

We intercept washing machines and dryers before landfill, restore and safety-certify them, and supply them to low-income households at a fair price — while running the workshop as a training floor for people locked out of the workforce.

> **A zero-waste local economy in which discarded household appliances are converted into community equity, environmental gain and secure local employment.**

**The model:** Intercept → Restore → Certify → Redistribute → Reinvest.

**Where we are:** Pre-launch. The 50-unit supply pilot is underway, and we're seeking founding supply, distribution and capability partners. [Read the prospectus →](https://circularappliances.com/prospectus)

The [impact dashboard](https://circularappliances.com/impact) currently reads zero on every measure. That is deliberate — the pilot has not yet produced a full month of operating records. We report what we actually achieved, including shortfalls, rather than publish a projection styled as a result. The numbers will fill in as the workshop runs.

---

## The standard I hold the work to

These aren't slogans on a wall. Each one has a test that can be checked.

| Principle | The test |
| :--- | :--- |
| **Safety** | "A second-hand appliance sold to a low-income family must be as safe as a new one." — 100% test-and-tag, named sign-off. |
| **Equity** | "Access to a working appliance should not depend on access to credit." — no credit checks, no compounding interest. |
| **Training** | "Training is paid, supervised and leads somewhere real." — wages are a cost of goods, not an afterthought. |
| **Honesty** | "We report what we actually achieved, including shortfalls." |

> "We are not asking funders to subsidise a service forever. We are asking them to fund the workshop that makes the service pay for itself."
>
> — Mark & Hayden Della Casa Alberighi, founding directors

---

## The platform

One codebase, two applications, one database — deployed on Cloudflare Workers via OpenNext.

- **Public website** — shop with three pricing tiers, concession and referral pathways, collection bookings, live impact reporting, and a partnership prospectus that prints to PDF for funders and councils.
- **Operations dashboard** — the workshop end to end: intake, triage, repair logging, AS/NZS 3760 testing with supervisor sign-off, listings, sales, rentals, warranty claims, trainee hours and partner pipeline.
- **Integration hub** — Stripe, email, SMS, Slack, signed outbound webhooks and a key-authenticated REST API, with credentials encrypted at rest.

**Engineering decisions I made that matter:**

- A unit cannot be listed without a **passed AS/NZS 3760 test signed off by a licensed supervisor** — refused in the state machine, not left to a manual.
- Every unit is serialised (`CAC-0001…`) and carries its test record, repair history and warranty claims for life.
- Impact figures come from operating records; closed periods are **frozen** so published numbers never move retrospectively.
- Money is integer cents in AUD. Concession evidence records card type sighted and expiry — never card numbers.
- Single-unit stock is claimed with compare-and-swap holds, so two buyers can never buy the same machine.

---

## Toolkit

![Next.js 15](https://img.shields.io/badge/Next.js_15-2C3539?style=flat-square&logo=nextdotjs&logoColor=F4F6F5)
![React 19](https://img.shields.io/badge/React_19-2C3539?style=flat-square&logo=react&logoColor=F4F6F5)
![TypeScript](https://img.shields.io/badge/TypeScript-2C3539?style=flat-square&logo=typescript&logoColor=F4F6F5)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-2C3539?style=flat-square&logo=tailwindcss&logoColor=F4F6F5)
![Prisma 6](https://img.shields.io/badge/Prisma_6-2C3539?style=flat-square&logo=prisma&logoColor=F4F6F5)
![Cloudflare Workers](https://img.shields.io/badge/Cloudflare_Workers-2C3539?style=flat-square&logo=cloudflare&logoColor=F4F6F5)
![Stripe](https://img.shields.io/badge/Stripe-2C3539?style=flat-square&logo=stripe&logoColor=F4F6F5)
![Zod](https://img.shields.io/badge/Zod-2C3539?style=flat-square&logo=zod&logoColor=F4F6F5)

Also Python, Node.js, Docker, Linux, DNS and self-hosted infrastructure. The platform is self-hostable end to end by design.

---

## Get in touch

- **Business:** [circularappliances.com](https://circularappliances.com) · [Partnership prospectus](https://circularappliances.com/prospectus) · [enquiries@circularappliances.com](mailto:enquiries@circularappliances.com)
- **Me directly:** [hayden@circularappliances.com.au](mailto:hayden@circularappliances.com.au)
- **Partnerships:** [Partners page](https://circularappliances.com/partners) — we are seeking capability capital, not an operating subsidy.

<div align="center">

<small>Brisbane, Australia · Divert waste · Restore value · Empower community</small>

</div>
