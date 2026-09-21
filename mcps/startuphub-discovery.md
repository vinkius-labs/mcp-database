# StartupHub Discovery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/startuphub-discovery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lead-generation](../categories/lead-generation.md)

Find startups before the press does — search 65M+ companies discovered from new domains, registries and GitHub orgs.

## Description
Connect **StartupHub.ai** to your AI agent and discover companies the way investors do: proactively, from the raw signals that appear *before* press coverage.

### What you can do

- **Search the discovered directory** — Filter 65M+ company profiles by country, sector, founding window, funding, stealth status and 40+ detected technology signals (CDN, hosting, email provider, payment processors, compliance certs, ATS, AI-support widgets)
- **Watch the domain radar** — Freshly registered .ai / .io names from NRD feeds, company registries and new GitHub orgs, with MX, parking and content-quality signals
- **Generate lists from a brief** — Describe an ICP in plain language (or paste a YC batch, a portfolio page or a CSV) and get a curated, directory-matched list of up to 50 startups
- **Read momentum** — Fastest-hiring companies, who is getting news and podcast buzz, and biggest AI-readiness score movers over 7/30/90 days
- **Get market context (0 credits)** — Weekly capital deployed, round counts, top sectors, countries, stages, notable rounds and exits
- **Track companies** — Create monitors that fire webhooks the moment a watched company raises, hires, changes stack or gets acquired

### Why this is different from web search

Web-search APIs answer "what was written about yesterday". StartupHub ingests new domain registrations, government registries (Israel, Canada, UK, US SEC Form D, France, …) and new GitHub orgs, probes the homepage, fingerprints the stack, and promotes a structured row — so you can ask "new cybersecurity startups in Israel this month" and get filterable rows, with pagination.

### How it works

1. Add this server to your agent
2. Add your **StartupHub API key** (Account → API) — required for every tool; anonymous calls are rejected with a payment challenge
3. Ask: "find stealth AI startups in Israel founded this month with verified founder emails"

### Who is this for?

- **VC analysts and scouts** — build and refresh deal-flow lists from signals that precede announcements
- **GTM and RevOps teams** — source companies by detected tech stack (Stripe + SOC 2 + Greenhouse = enterprise-ready B2B)
- **Market researchers** — weekly funding pulse and sector momentum with zero setup


## Available Tools (10)
- **market_trends**: Use it to open a prospecting conversation with market context.

Weekly snapshot of the AI startup market: capital deployed, rounds, top sectors, countries, stages and exits
- **monitor_company**: Costs 5 credits. Set webhook_url to receive {event, entity_id, title, body, metadata, delivered_at} the instant a change is detected; frequency is clamped to your plan (faster cadence needs a higher tier). Closes the discovery loop: find with search_startups, then track with this tool.

Watch a company and get notified the moment it raises, hires, changes stack or gets acquired
- **news_mentions**: Each entry links to the company profile and its latest mention title. Costs 2 credits. Orthogonal to search_startups — combine both: directory filters find the ICP, this tool finds who has momentum this week.

See which companies are getting news and podcast buzz, ranked by mention count
- **score_movers**: Costs 1 credit. direction=up surfaces companies improving their agent-readiness (good prospects for "you improved, here's what's next" outreach); direction=down flags decline.

Biggest AI-readiness score risers and fallers over the last 7, 30 or 90 days
- **search_domains**: These are NOT companies: no enrichment, no sectors. A startup_slug appears only once the homepage passes quality review and a public profile is published — then switch to search_startups. Default status is "queued,quality_failed" (names still being watched). Costs 1 credit.

Watch freshly registered domains (the raw radar) before they become company profiles
- **submit_startup**: Strict format: third-person prose, no HTML or markdown, no listicle words ("best", "top", "2026") in the name. On invalid input the API returns 400 with field-level errors and copy-paste suggestions — fix those exact fields and resubmit. A 409 means the domain already has a profile: do not resubmit. sectors_json must hold 1-5 sectors. Free tier allows 10 submissions/day.

Submit a new company for inclusion in the StartupHub.ai directory
- **trending_hiring**: Costs 1 credit. Use it to pre-qualify a search_startups result list — companies actively scaling are warmer outreach targets.

Rank companies by how fast they are adding open roles right now
- **sector_trends**: Use after market_trends to drill into a sector that attracted capital this week.

Funding momentum and company counts for a sector, or resolve one company to its sectors
- **ai_generate_list**: The engine runs a grounded web search, parses results and matches them to the directory, returning up to 50 startups. Costs 5 credits, with a burst limit of 10 calls per 10 minutes. On 502/504, retry with a more specific prompt. Requires an API key.

Turn a natural-language brief into a curated list of matching startups
- **search_startups**: Each row returns name, slug, one-liner, website, HQ, founded date, sectors, score and detected tech fingerprint; paginate with limit/offset (total shown in the response). Costs 1 credit. Two different "new" timestamps: sort=created_at.desc means added to the directory this week; founded_after/founded_before filter by the company's own founding date.

Search 65M+ proactively discovered companies by sector, country, funding, stealth and 40+ detected tech signals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **StartupHub Discovery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find new cybersecurity startups in Israel founded in the last three months."

**🤖 AI Agent:**
> I ran search_startups with country=Israel, sector=Cybersecurity, founded_after=2026-06-17, sort=created_at.desc. 38 companies matched; the top of the list by directory score is Orca Security spin-out "Nexus Threat" (founded 2026-07-02, 12 employees, Cloudflare + Google Workspace, SOC 2 badge detected). Page 1 of 2 — say the word and I'll fetch offset=25.

---

**👤 You:**
> "What's the AI startup market doing this week, and which sector is hot?"

**🤖 AI Agent:**
> market_trends shows $12.4B deployed across 50 rounds this week (-10.6% WoW), 72 new startups and 10 exits. The hottest sector by capital is Tunneling Infrastructure ($3.0B, one round: The Boring Company Series D), followed by SpaceTech ($2.5B, Cohere Series E). Want me to drill into sector trends for any of these?


## ❓ FAQ

**Q: Do I need an API key?**
Yes — every tool requires an sk_live_ key. Create one at https://www.startuphub.ai/my-account?tab=api. Without a key the API answers anonymous calls with an x402 payment challenge instead of data, so the connector asks for the key up front.

**Q: How are credits charged?**
Each call spends credits from the plan's daily allowance: 1 for a search or domain-radar page, 2 for news mentions, 5 for an AI-generated list or a monitor. Market trends, sector trends and submissions are free (10 submissions/day on the free tier). Responses include the remaining balance so the agent can budget.

**Q: How is this different from StartupHub's own MCP server?**
StartupHub's hosted MCP exposes only a handful of free utilities (logo lookup, email validation, trends). This server covers the discovery half of the paid API — directory search with all 40+ filters, the domain radar, AI-generated lists, hiring and news momentum, score movers and monitors — with normalized pagination and credit-aware responses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/startuphub-discovery](https://vinkius.com/en/ai-agent-connect/startuphub-discovery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **StartupHub Discovery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `startuphub-discovery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **StartupHub Discovery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "startuphub-discovery": {
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
