# StartupHub People & Intel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/startuphub-people-intel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lead-generation](../categories/lead-generation.md)

Find founders and investors, discover verified professional emails, and unlock deep-intelligence dossiers.

## Description
Connect **StartupHub.ai** to your AI agent and work the people side of deal-flow and outreach: find who runs a company, get a verified way to reach them, and pull a regulatory-grade dossier when the stakes are high.

### What you can do

- **Find people** — Search founders, executives, board members and key team members by name, title, country, sector or tags (Unit 8200, Serial Entrepreneur, Has Exits)
- **Resolve anyone** — One tool for slug, email or LinkedIn/X handle lookups; no more guessing which endpoint fits which identifier
- **Find verified emails** — Give a name and a company domain, get back a deliverable address; verify an address you already have; or turn a single email into a person plus their company
- **Find investors** — Search VCs, angels, accelerators and CVCs, then match a startup to its best-fit investors by sector overlap, activity and stage
- **Preview deep intelligence (free, no key)** — See exactly which dossier sections exist for a person or company before spending a credit
- **Unlock full dossiers** — Regulatory and corporate filings, ownership and control structures, fund assets under management, compensation benchmarks and verified contacts, every section unredacted
- **Score agent readiness** — Scan any site for AI-agent readiness; the failed checks are ready-made outreach hooks

### How it works

1. Add this server to your agent
2. Optionally add your **StartupHub API key** (Account → API) — intel previews are free without one; people, emails, matching and dossiers need it
3. Ask: "find the CTO of that cybersecurity startup and get me their verified email"

### Who is this for?

- **Founders fundraising** — build an investor list ranked by real fit, not logo bias
- **Recruiters and sourcers** — reach founders and executives with verified contacts
- **Sales and partnerships** — identify the right person and a deliverable email in two calls
- **Risk and compliance teams** — deep dossiers from authoritative public records


## Available Tools (11)
- **discover_email**: Costs 3 credits. If the first attempt returns no match, retry once with the same arguments — the first call sometimes warms the lookup cache. Do not chain validate_email behind this tool: discovery already validates every candidate it returns.

Find a professional email address for a person, given their name and company domain
- **enrich_email**: Costs 5 credits. When the person is unknown it returns a best-guess name derived from the address — treat unverified names as a hypothesis, not a fact. The natural pair: enrich_email opens the conversation, then company_funding in the enrich server deepens the account.

Turn one email address into a person plus their company context
- **get_person**: Costs 1 credit. Full contact fields are plan-gated; the response includes whatever your tier allows. For an email you already have, enrich_email gives you the person AND their company in one call (5 credits).

Fetch a person by slug, email or social handle — one tool for all three lookups
- **intel_lookup**: Compiles regulatory and corporate filings, financial ownership and control structures, fund assets under management, compensation benchmarks by role, affiliated entities and verified contacts — from authoritative public records, with people automatically linked to the companies and funds they control. Run intel_preview first: it is free and shows exactly which sections will be populated, so you never spend 10 credits on an empty dossier.

Full deep-intelligence dossier on any person or company, every section unredacted
- **intel_preview**: Pass any identifier — a name, a company, a domain, a LinkedIn URL or an email. Returns who was resolved and which sections exist (regulatory filings, ownership and control, fund assets, compensation benchmarks, affiliated entities, verified contacts) with a teaser, but not the values. Use it to check whether a dossier is worth unlocking before spending 10 credits on intel_lookup.

Preview a deep-intelligence dossier: identity plus a manifest of available sections. Free, no key
- **match_investors**: Returns ranked matches with a fit score and a breakdown of sector overlap, activity and stage. Costs 1 credit. This is the fundraising workflow: find your startup with search_startups (discovery server) or resolve_company (enrich server), then match it to investors here.

Find the best-fit investors for a startup — or the best-fit startups for an investor
- **scan_agent_readiness**: txt, llms.txt, structured data, crawlability and content depth, then returns a score, a letter grade and a per-check breakdown where each failure carries a copy-paste fix prompt. The outreach hook: failed checks are exactly what to lead with ("your site scores 23/100 for agents, here is what is missing"). Free with an API key; without one the API demands per-call crypto payment.

Score any website 0-100 for AI-agent readiness, with per-check fix prompts
- **get_investor**: Costs 1 credit. Returns type, sector and stage focus, cheque size, portfolio and funds (fields scale with plan tier).

Fetch an investor record by slug, website domain or social handle
- **search_investors**: Costs 1 credit. Slugs from here feed get_investor for cheque size, sector/stage focus and portfolio.

Search VCs, angels, accelerators, corporate and PE investors by name, country or type
- **search_people**: Each result returns name, slug, title, city, country, sectors, score and tags (e.g. "Unit 8200", "Serial Entrepreneur", "Has Exits"). Costs 1 credit, paginated with limit/offset. Slugs from here feed get_person; combine with discover_email in this server to reach out.

Search founders, executives and key team members by name, title, country, sector or tag
- **validate_email**: Costs 1 credit. Do not run this on the output of discover_email — discovery validates internally and double-validating only wastes credits.

Verify whether a single email address is real and deliverable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **StartupHub People & Intel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the CEO of Anthropic and get me a verified email."

**🤖 AI Agent:**
> search_people found Dario Amodei (slug `dario-amodei`, "CEO and Co-founder at Anthropic"). discover_email with firstName=Dario, lastName=Amodei, domain=anthropic.com returned [email protected] with confidence 95. The address is deliverable — discovery validates internally, so no extra verification call needed.

---

**👤 You:**
> "Which investors are the best fit for our startup, acme-security.com?"

**🤖 AI Agent:**
> resolve_company (enrich server) gave me your slug `acme-security` — Cybersecurity, Israel, seed stage. match_investors ranked 12 investors: top fit is Example Ventures (82 — sector overlap 40, activity 30, stage 12), which closed 4 rounds in the last 90 days. Want me to pull its cheque size and portfolio focus with get_investor?


## ❓ FAQ

**Q: How is this different from StartupHub's own MCP server?**
StartupHub's hosted MCP exposes only a few free utilities. This server covers the people, investor and intelligence half of the API — people search, multi-identifier resolution, email discovery and verification, investor matching, and the deep-intelligence dossiers — with unified lookups so you never have to pick the right endpoint.

**Q: Should I use discover_email or validate_email?**
`discover_email` goes from a name + company domain to a found, verified address (3 credits) and already validates every candidate internally. `validate_email` (1 credit) is only for an address you already have from somewhere else — a contact page, a signature, a scraped profile. Running validate on discover output wastes credits.

**Q: What is a deep-intelligence dossier and what does it cost?**
It is a compiled dossier on a person or company from authoritative public records: regulatory and corporate filings, ownership and control structures, fund assets under management, compensation benchmarks, affiliated entities and verified contacts. Each lookup costs 10 credits, so run the free `intel_preview` first — it shows exactly which sections will be populated, so you never pay for an empty dossier.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/startuphub-people-intel](https://vinkius.com/en/ai-agent-connect/startuphub-people-intel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **StartupHub People & Intel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `startuphub-people-intel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **StartupHub People & Intel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "startuphub-people-intel": {
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
