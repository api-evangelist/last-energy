# Last Energy

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
