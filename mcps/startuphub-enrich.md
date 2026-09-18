# StartupHub Enrich MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/startuphub-enrich)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Turn any domain into a full company dossier: funding, revenue, tech stack, hiring, news mentions and Reddit sentiment.

## Description
Connect **StartupHub.ai** to your AI agent and enrich any company from its website alone — the way enrichment should work: one identifier in, a full dossier out.

### What you can do

- **Resolve any identifier** — A domain *or* a LinkedIn company URL becomes a full record: name, slug, sectors, HQ, funding, headcount and score. Domains cost 1 credit, LinkedIn 3
- **Batch-enrich a CRM export** — Up to 100 domains per call, each echoing a matched flag so you know exactly which rows need a follow-up enrichment
- **Deepen a profile on demand** — Run the grounded enrichment pipeline (live search grounding, site scrape, tech fingerprint, LinkedIn/jobs/GitHub passes) to create or refresh a company
- **Read the numbers** — Funding snapshot (total raised, latest round, valuation, fundraising status, capital efficiency) and estimated revenue with a clear verified-vs-estimate flag
- **See the stack** — Detected CDN, hosting, email provider, frameworks, payments and analytics, with a fingerprint timestamp
- **Read the signals** — Hiring velocity with a sample of live open roles, news and podcast mentions with quotes, and public Reddit sentiment
- **Score trust (free, no key)** — A 0-100 trust and reputation score with per-signal breakdown, plus an Effective Domain Rating that shows whether a brand is over- or under-rated vs its Ahrefs DR

### How it works

1. Add this server to your agent
2. Optionally add your **StartupHub API key** (Account → API) — trust and domain-rating scans work without one, the rest needs it
3. Ask: "what do you know about ramp.com?"

### Who is this for?

- **RevOps and data teams** — enrich CRM rows from a website field instead of manual research
- **Sales engineers** — walk into a call knowing the prospect's funding, stack and hiring plan
- **Vendor-risk analysts** — trust scores and reputation findings before signing


## Available Tools (12)
- **company_funding**: Costs 1 credit. Ideal for enriching a single CRM row from its website.

Funding snapshot for one company by domain: total raised, latest round, valuation, fundraising status
- **company_mentions**: Each mention carries its publication, date, a quote and an importance grade; counts summarise news vs podcast. Costs 1 credit. Good for pre-meeting prep or for spotting a narrative shift; for who-is-hot-this-week across all companies use news_mentions in the discovery server.

News and podcast mentions for one company, with quotes and importance grades
- **company_revenue**: Costs 1 credit. Treat unverified estimates as directional, not fact — the response says which is which.

Estimated revenue for one company by domain, with verification status and revenue per employee
- **company_technology**: Costs 1 credit. Use it to qualify buyers (e.g. a Greenhouse ATS + SOC 2 badge suggests a mature hiring process) or to find lookalike stacks.

Detected technology stack for one company by domain — CDN, hosting, email provider, frameworks, payments, analytics
- **effective_domain_rating**: Compares a domain's effective rating against its Ahrefs DR and returns an "underrated" or "overrated" verdict, with per-surface scores (search visibility, brand mentions, AI citations, web health). Useful when qualifying marketing-tool prospects: a high EDR with a low DR means real attention that link metrics miss.

Effective Domain Rating (0-100): realized cross-surface visibility vs the classic Ahrefs DR
- **enrich_company**: Runs live search grounding, a website scrape, tech fingerprinting and LinkedIn/jobs/GitHub passes, and creates a pending stub if the company is not on file yet. Costs 5 credits and needs Pro Lite or higher. Set fast=true to read the cached row only (no pipeline, no fresh cost); force=true to re-run even if enriched within the last 7 days. This deepens a row you already found — to discover net-new companies use search_startups instead.

Run the full grounded enrichment pipeline on a known company and return its profile
- **get_startup**: g. "anthropic"). Costs 1 credit. Returned fields scale with plan tier: free returns basics, paid returns everything including stealth details.

Fetch the full profile of one startup by its StartupHub slug
- **hiring_scan**: Costs 2 credits. The sample titles tell you what a company is building — a run of "Account Executive" hires means a sales motion, "ML Engineer" hires mean product investment.

Hiring signal for one company: open-role count, recent velocity and a sample of live roles
- **reddit_reviews**: Costs 1 credit. Real-user complaints are gold for qualification and for objection handling in outreach.

Public Reddit sentiment and review snippets for one company
- **resolve_company**: com) or a LinkedIn company URL/handle, get back name, slug, website, one-liner, sectors, HQ, funding, employee count and score. Domain lookups cost 1 credit; LinkedIn lookups cost 3 because they can live-fetch from LinkedIn — prefer the domain when you have it. A 404 means no company matched: fall back to search_startups in the discovery server, or enrich_company to create the profile.

Resolve a website domain or a LinkedIn company page to a full StartupHub company record
- **trust_reputation**: Scores security posture (HSTS, CSP, headers), privacy transparency (policy presence, GDPR/CCPR mentions), a Safe Browsing malware check and publicly reported reputation/legal findings, each with its own subscore. Great as a pre-outreach sanity check or a vendor-risk signal.

Trust and reputation score (0-100) for any domain, with a per-signal breakdown
- **bulk_match_domains**: Costs 1 credit per call regardless of batch size. Unmatched domains are not errors — collect them and run enrich_company on the ones that matter.

Batch-resolve up to 100 domains to company records in one call — for enriching a CRM export


## 💬 Prompt Examples

Here are some examples of how you can interact with the **StartupHub Enrich** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What do you know about ramp.com?"

**🤖 AI Agent:**
> resolve_company on ramp.com → Ramp (slug `ramp`), corporate cards and spend management, Fintech, United States, ~$1.9B raised, ~1000 employees, score 84. Want the funding detail, the tech stack and hiring signal too? That's three more 1-2 credit calls.

---

**👤 You:**
> "Enrich these 40 domains from our CRM export and tell me which ones have no profile."

**🤖 AI Agent:**
> bulk_match_domains resolved all 40 in one call: 31 matched (Ramp, Anthropic, Cursor...), 9 have no profile on file. I ran enrich_company on the 3 you flagged as strategic; the rest are queued for your review.


## ❓ FAQ

**Q: What's the difference between resolve_company and enrich_company?**
`resolve_company` reads the existing directory record (1 credit for a domain, 3 for LinkedIn). `enrich_company` runs the full pipeline — live search grounding, a site scrape, tech fingerprinting and LinkedIn/jobs/GitHub passes — and creates the company if it does not exist yet (5 credits). Read first; enrich only when the read is missing or stale.

**Q: Is the revenue figure reliable?**
The response marks it explicitly: `is_revenue_verified` tells you whether the estimate was grounded in a verified source or is a model estimate. Treat unverified values as directional and say so when you quote them.

**Q: Do I need an API key?**
It is optional. `trust_reputation` and `effective_domain_rating` are free public tools that work with no key. Profile lookups, enrichment, funding, revenue, tech, hiring and mentions require an sk_live_ key — create one at https://www.startuphub.ai/my-account?tab=api.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/startuphub-enrich](https://vinkius.com/en/ai-agent-connect/startuphub-enrich)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **StartupHub Enrich** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `startuphub-enrich` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **StartupHub Enrich** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "startuphub-enrich": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
