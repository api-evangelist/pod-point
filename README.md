# Pod Point

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Pod Point — trading as Pod since its February 2026 rebrand, with pod-point.com now 301-redirecting to podenergy.com — is a British electric vehicle charging company founded in London in 2009 and wholly owned by EDF since its delisting from the London Stock Exchange in August 2025. It sells and installs home, workplace and fleet chargers, operates the third-largest public charging network in the United Kingdom across Tesco and Lidl car parks, and acquired depot-charging specialist EO Charging in May 2026. It sits on the demand side of the UK electricity value chain, between the driver and the electricity supplier, as a Charge Point Operator rather than a metering, network or settlement body. Its API posture is narrow but real and honestly split: there is no developer portal, no OpenAPI, no Swagger and no consumer data API, yet a live OCPI 2.2.1 Charge Point Operator service runs at ocpi.podenergy.com whose version negotiation answers anonymously and enumerates a full module set, while every data module — locations, tariffs, sessions, CDRs — returns 401 Unauthorized without a bilaterally exchanged OCPI credentials token. Britain's Public Charge Point Regulations 2023 name OCPI 2.2.1 as the vehicle for open charge point data; the plumbing that regulation names is verifiably in place at Pod, but the open part of it is not obtainable anonymously from outside, and the company publishes no open data page, no OCPI token policy and no developer onboarding of any kind.

**Areas:** Energy · United Kingdom · EV Charging · Electric Vehicles · Utilities · Electricity · OCPI · Charge Point Operator · Smart Charging · Grid

## Pod Point on APIs.io

Everything profiled for Pod Point is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/pod-point/](https://apis.io/providers/pod-point/)** — or go straight to one of the APIs or properties below.

### APIs (1)

- [Pod OCPI 2.2.1 CPO API](https://apis.io/apis/pod-point/pod-point-ocpi-cpo-api/) — Pod's Open Charge Point Interface (OCPI) 2.2.1 service in the Charge Point Operator role, used for e-mobility roaming and as the technical vehicle named by…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Examples (4)

Example requests and responses.

- [Pod Point Ocpi Health](https://apis.io/examples/pod-point/pod-point-ocpi-health/)
- [Pod Point Ocpi Unauthorized](https://apis.io/examples/pod-point/pod-point-ocpi-unauthorized/)
- [Pod Point Ocpi Version Detail](https://apis.io/examples/pod-point/pod-point-ocpi-version-detail/)
- [Pod Point Ocpi Versions](https://apis.io/examples/pod-point/pod-point-ocpi-versions/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Pod Point Authentication](https://apis.io/security/pod-point/pod-point-authentication/)
- [Pod Point Domain Security](https://apis.io/security/pod-point/pod-point-domain-security/)
- [Pod Point Vulnerability Disclosure](https://apis.io/security/pod-point/pod-point-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://podenergy.com/)
- [Support](https://help.pod-point.com/)
- [Blog](https://podenergy.com/news)
- [Security](https://podenergy.com/security)
- [Terms of service](https://podenergy.com/general-terms-and-conditions)
- [Privacy policy](https://podenergy.com/legal/privacy-notice)
- [GitHub](https://github.com/Pod-Point)

## API Evangelist rating

**Kin Score 26.8** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 6.5 |
| Contract governance | 18.2 |
| Operational transparency | 13.2 |
| Developer ergonomics | 39.3 |
| Access clarity | 21.1 |

**Agent readiness 4.5** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 25.4** — Energy & Utilities

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/pod-point/](https://apis.io/providers/pod-point/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Pod Point: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/pod-point/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
