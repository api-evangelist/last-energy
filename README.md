# Last Energy

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

Last Energy is an American developer and operator of micro-modular nuclear power plants, founded in 2019 in Washington, D.C. by Bret Kugelmass as a commercial spinout of the Energy Impact Center. Its PWR-20 is a 20 MWe pressurized water reactor assembled from a few dozen factory-made, steel-encased modules that ship to site and are installed rather than constructed in place.

Last Energy sells power, not reactors: it designs, finances, owns and operates plants under long-term power purchase agreements for energy-intensive customers including data centers, metals, chemicals, cement, pulp and paper, and food and beverage. It has announced projects in Texas, South Wales, Poland and Romania, entered nuclear site licensing in the United Kingdom, and raised roughly $164M across a $40M Series B and a $100M Series C.

## API surface

**None found.** Contract discovery on 2026-08-01 found no public API, developer portal, SDK, CLI, MCP server, or agent card:

- `/openapi.json`, `/swagger.json`, `/api-docs`, `/llms.txt` — all HTTP 404 on `www.lastenergy.com`
- The entire `/.well-known/*` surface returns the Webflow placeholder `Invalid .well-known request` (404), including `agent-card.json` and `agent.json`
- No `api.`, `developer.`, `docs.`, `app.`, `portal.`, `status.`, `trust.` or `mcp.` subdomain resolves in DNS
- No first-party packages on npm, PyPI, or the other registries
- The 572-URL sitemap contains only marketing, news, careers, and gated-portal pages

The only authenticated surface is a Webflow customer account (`/sign-up`, `/log-in`, `/user-account`) used to gate whitepapers and regional portals. It exposes no programmatic interface.

## Artifacts

- `security/last-energy-domain-security.yml` — probed TLS 1.3, HSTS (1 year), DNSSEC enabled, SPF and DMARC (`quarantine`), no CAA record
- `well-known/last-energy-well-known.yml` — recorded negative result for the `/.well-known/` discovery surface
- `llms/last-energy-llms.txt` — generated llms.txt for the company's public surface

## Links

- https://www.lastenergy.com/
- https://en.wikipedia.org/wiki/Last_Energy
- https://forgeglobal.com/last-energy_stock/
