# Red 6

Red 6 (Red Six Aerospace, Inc.) is a defense technology company founded in 2018 that builds outdoor,
high-speed augmented reality for military aviation training. Its flagship product, **ATARS** (Advanced
Tactical Augmented Reality System), pairs the **EVE** (Enhanced Visual Environment) helmet-mounted
display — 160-degree field of view, 18,000 nits, 10ms latency, full color — with an AI-driven
multiplayer network so real pilots in real aircraft can fly and maneuver against synthetically
generated adversaries in real time, in daylight. A companion system, **ARCADE** (Augmented Reality
Command and Analytic Data Environment), handles mission planning, briefing and 3D debrief.

ATARS has been integrated or trialed on the USAF F-16 and MC-130, the RAF Hawk T-2, Boeing's AH-64E
Apache CATT, and the Lockheed Martin / Korea Aerospace Industries T-50 and TF-50.

- Website: https://red6ar.com/
- ATARS: https://red6ar.com/atars/
- Newsroom: https://red6ar.com/newsroom/
- ISO 9001:2015 and AS9100D: https://red6ar.com/iso-90012015-and-as9100d/
- Secondary market (Forge Global): https://forgeglobal.com/red6_stock/

## API surface

**None published.** As of the 2026-08-02 enrichment pass, Red 6 publishes no public API, SDK,
developer portal, changelog, status page, or machine-readable contract. Every contract-discovery probe
missed on `red6ar.com` and `www.red6ar.com`, and `api.`, `developer.`, `docs.`, `dev.`, `arcade.`,
`status.`, `trust.` and `portal.red6ar.com` do not resolve:

| Probe | Result |
|---|---|
| `/openapi.json`, `/openapi.yaml`, `/swagger.json`, `/api-docs` | 404 / 403 (WordPress shell) |
| `/llms.txt` | 404 |
| `/.well-known/security.txt` | 404 |
| `/.well-known/openid-configuration`, `/oauth-authorization-server`, `/oauth-protected-resource` | 404 |
| `/.well-known/api-catalog`, `/ai-plugin.json`, `/mcp.json` | 404 |
| `/.well-known/agent-card.json`, `/.well-known/agent.json` | 404 |
| GraphQL / MCP endpoints | none advertised anywhere in docs or site |

Red 6's software is delivered through defense programs and OEM aircraft integrations, not a self-serve
developer platform. `github.com/red6` belongs to **red6 enterprise software GmbH** (a Hamburg insurance
software company) and is *not* this company — do not wire it as a GitHub organization.

## Artifacts in this repo

| Artifact | File | Method |
|---|---|---|
| Conformance / certifications | `conformance/red6-conformance.yml` | searched |
| Domain security | `security/red6-domain-security.yml` | probed |
| Well-known discovery record | `well-known/red6-well-known.yml` | probed (all 404) |
| llms.txt | `llms/red6-llms.txt` | generated |
