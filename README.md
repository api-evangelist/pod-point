# Pod Point (pod-point)

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

Pod Point — trading as Pod since its February 2026 rebrand, with pod-point.com now 301-redirecting to podenergy.com — is a British electric vehicle charging company founded in London in 2009 and wholly owned by EDF since its delisting from the London Stock Exchange in August 2025. It sells and installs home, workplace and fleet chargers, operates the third-largest public charging network in the United Kingdom across Tesco and Lidl car parks, and acquired depot-charging specialist EO Charging in May 2026. It sits on the demand side of the UK electricity value chain, between the driver and the electricity supplier, as a Charge Point Operator rather than a metering, network or settlement body. Its API posture is narrow but real and honestly split: there is no developer portal, no OpenAPI, no Swagger and no consumer data API, yet a live OCPI 2.2.1 Charge Point Operator service runs at ocpi.podenergy.com whose version negotiation answers anonymously and enumerates a full module set, while every data module — locations, tariffs, sessions, CDRs — returns 401 Unauthorized without a bilaterally exchanged OCPI credentials token. Britain's Public Charge Point Regulations 2023 name OCPI 2.2.1 as the vehicle for open charge point data; the plumbing that regulation names is verifiably in place at Pod, but the open part of it is not obtainable anonymously from outside, and the company publishes no open data page, no OCPI token policy and no developer onboarding of any kind.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/pod-point/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/pod-point/refs/heads/main/apis.yml)

## Tags

- Energy
- United Kingdom
- EV Charging
- Electric Vehicles
- Utilities
- Electricity
- OCPI
- Charge Point Operator
- Smart Charging
- Grid

## Timestamps

- **Created:** 2026-07-27
- **Modified:** 2026-07-27

## APIs

### Pod OCPI 2.2.1 CPO API

Pod's Open Charge Point Interface (OCPI) 2.2.1 service in the Charge Point Operator role, used for e-mobility roaming and as the technical vehicle named by the UK Public Charge Point Regulations 2023 for charge point reference and availability data. Version discovery is anonymous: `GET /ocpi/cpo/versions` returned HTTP 200 on 2026-07-27 advertising version 2.2.1, and `GET /ocpi/cpo/2.2.1` returned HTTP 200 enumerating `cdrs`, `credentials`, `locations`, `sessions` and `tariffs` in the SENDER role plus `commands`, `credentials` and `tokens` in the RECEIVER role. Every one of those data modules returns HTTP 401 with OCPI `status_code` 2000 Unauthorized to an anonymous caller; access requires an OCPI credentials token exchanged bilaterally with Pod. Pod publishes no human documentation, no OpenAPI and no onboarding path for this API — the module list the service returns about itself is the only contract.

- **Human URL:** [https://ocpi.podenergy.com/ocpi/cpo/versions](https://ocpi.podenergy.com/ocpi/cpo/versions)
- **Base URL:** `https://ocpi.podenergy.com/ocpi/cpo/2.2.1`

#### Tags

- EV Charging
- OCPI
- Roaming
- Charge Point Operator
- Open Data
- United Kingdom

#### Properties

- [API Reference](https://ocpi.podenergy.com/ocpi/cpo/versions)
- [Documentation](https://github.com/ocpi/ocpi)
- [Specification](https://evroaming.org/wp-content/uploads/2024/11/OCPI-2.2.1-d2.pdf)
- [Regulation](https://www.legislation.gov.uk/uksi/2023/1168/contents/made)

## Common Properties

- [Website](https://podenergy.com/)
- [Blog](https://podenergy.com/news)
- [Support](https://help.pod-point.com/)
- [GitHub Organization](https://github.com/Pod-Point)
- [LinkedIn](https://www.linkedin.com/company/podpoint)
- [Careers](https://careers.pod-point.com/)
- [Security](https://podenergy.com/.well-known/security.txt)
- [Terms of Service](https://podenergy.com/general-terms-and-conditions)
- [Privacy Policy](https://podenergy.com/legal/privacy-notice)

## Maintainers

- **Kin Lane** — kin@apievangelist.com
