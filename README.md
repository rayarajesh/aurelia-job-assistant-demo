# Aurelia — Personal AI Job Hunting Assistant Demo

A dependency-free, client-facing proof-of-concept website based on the October 2, 2026 requirements brief.

## Run locally

From this directory, run any static server:

```bash
python3 -m http.server 4173
```

Then open <http://localhost:4173>.

You can also use VS Code Live Server or any other static-file server. No npm install or external service is required for this demo.

## What is included

- Command center with pipeline, KPIs, system health, and outbound protection
- Four synthetic demo candidate workspaces: Aman Reddy, Priya Nair, Mateo Santos, and Sarah Kim, each with separate sample metrics, roles, jobs, applications, resumes, and messages
- Opportunity discovery, screening, fit dimensions, source evidence, exclusions, and holds
- Integrations & APIs map covering n8n, public job feeds, backend REST/JSON, PostgreSQL, LLM adapters, DOCX/PDF storage, Playwright, Google Sheets, and Gmail later
- Review queue for approvals, missing facts, duplicate reconciliation, and receipt checks
- Resume/evidence review with exact artifact metadata and SHA-256 manifest
- Application pipeline with approval binding, uncertain outcomes, and receipt verification
- Recruiter communications workspace with verified-fact drafts, recipient purpose, rate clarification, follow-up defaults, and suppression controls
- Google Sheets-style tracking view with sync simulation and manual-note preservation
- Audit timeline and architecture/data-flow view
- Demo lab covering Meta/Delart exclusions, Arista referral hold, missing facts, hostile content, deduplication, changed descriptions, uncertain submissions, and matching receipts

## Important demo boundary

This is a frontend demonstration with deterministic mock data and simulated interactions. It includes four synthetic candidate personas for client demonstrations, but the production requirements brief is scoped to one personal owner. It does not connect to n8n, Postgres, Google Sheets, an LLM provider, a live job source, a portal, or an outbound messaging channel. The UI intentionally keeps outbound protection enabled by default to demonstrate the owner-approval model described in the requirements.
