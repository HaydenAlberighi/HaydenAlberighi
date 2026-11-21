<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:061F17,100:1B7A5E&height=170&section=header&text=Hayden%20Della%20Casa%20Alberighi&fontSize=52&animation=fadeIn" />

# Hayden Della Casa Alberighi

**Director & Engineer — [Circular Appliance Co.](https://circularappliances.com)** · Brisbane, Australia

[![Role](https://img.shields.io/badge/Director_%26_Engineer-0F4C3A?style=flat-square)](https://circularappliances.com/about#governance)
[![Location](https://img.shields.io/badge/Brisbane%2C_Australia-2C3539?style=flat-square)](#)
[![Status](https://img.shields.io/badge/Pre_launch%E2%80%94seeking_founding_partners-D4AF37?style=flat-square)](https://circularappliances.com/partners)

---

### Circular Appliance Co.

A Brisbane social enterprise that intercepts washing machines and dryers before
landfill, restores them to certified safety standards, and supplies them to
low-income households at a fair price — while running the workshop as a
supported training floor that moves people into paid trade work.

> **Divert waste · Restore value · Empower community**

As a director I hold governance and commercial accountability; as the developer
I designed and built the entire platform; and in operations I run the workshop
end to end — intake through refurbishment, safety certification, sales and
impact reporting.

| Area | Responsibility |
| :--- | :--- |
| **Governance** | Director — commercial model, partnerships, compliance posture |
| **Engineering** | Public website, operations dashboard, integration hub, REST API |
| **Operations** | Workshop workflow, pricing, partner pipeline, impact measurement |

---

### The platform I built

One codebase, two applications, one database — deployed on Cloudflare Workers
via OpenNext:

- **Public website** — shop with three pricing tiers, concession and referral
  pathways, collection bookings, live impact reporting, and a partnership
  prospectus that prints to PDF for funders and councils.
- **Operations dashboard** — the workshop end to end: intake, triage, repair
  logging, AS/NZS 3760 safety testing with licensed supervisor sign-off,
  listings, sales, rentals, warranty claims, trainee hours and partner pipeline.
- **Integration hub** — Stripe, email, SMS, Slack, signed outbound webhooks and
  an API-key-authenticated REST API, with credentials encrypted at rest.

**Engineering principles the code enforces:**

- A unit cannot be listed for sale without a **passed AS/NZS 3760 test signed
  off by a licensed supervisor** — refused in the state machine, not the manual
- Every unit serialised (`CAC-0001…`) carrying its test record, repair history
  and warranty claims for life
- Impact figures computed from operating records; closed periods **frozen** so
  published numbers never move retrospectively
- Money handled as integer cents in AUD; concession evidence stored as card
  type sighted + expiry — never card numbers
- Single-unit stock claimed via compare-and-swap holds, so two buyers can never
  buy the same machine

---

### Toolkit

![Next.js 15](https://img.shields.io/badge/Next.js_15-2C3539?style=flat-square&logo=nextdotjs&logoColor=F4F6F5)
![React 19](https://img.shields.io/badge/React_19-2C3539?style=flat-square&logo=react&logoColor=F4F6F5)
![TypeScript](https://img.shields.io/badge/TypeScript-2C3539?style=flat-square&logo=typescript&logoColor=F4F6F5)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-2C3539?style=flat-square&logo=tailwindcss&logoColor=F4F6F5)
![Prisma](https://img.shields.io/badge/Prisma_6-2C3539?style=flat-square&logo=prisma&logoColor=F4F6F5)
![Cloudflare Workers](https://img.shields.io/badge/Cloudflare_Workers-2C3539?style=flat-square&logo=cloudflare&logoColor=F4F6F5)
![Stripe](https://img.shields.io/badge/Stripe-2C3539?style=flat-square&logo=stripe&logoColor=F4F6F5)
![Zod](https://img.shields.io/badge/Zod-2C3539?style=flat-square&logo=zod&logoColor=F4F6F5)

Also in the toolbox: Python, Node.js, Docker, Linux, DNS and self-hosted
infrastructure — the platform is self-hostable end to end by design.

---

### Connect

- 🏭 **Business:** [circularappliances.com](https://circularappliances.com) · [Partnership prospectus](https://circularappliances.com/prospectus) · [enquiries@circularappliances.com](mailto:enquiries@circularappliances.com)
- ✉️ **Direct:** [hayden@circularappliances.com.au](mailto:hayden@circularappliances.com.au)

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:1B7A5E,100:061F17&height=90&section=footer&animation=fadeIn" />
