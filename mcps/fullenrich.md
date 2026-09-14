# FullEnrich MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fullenrich)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Find verified work emails, personal emails and mobile numbers across 25+ data vendors with one waterfall.

## Description
Connect your **FullEnrich** account to any AI agent and enrich B2B contacts the way growth teams do: run a waterfall across 25+ data vendors, pay credits only when verified data is found, and get the most probable work email, personal email and mobile number for each prospect.

### What you can do

- **Waterfall Enrichment** — Submit up to 100 contacts by name + company (or LinkedIn URL) and retrieve verified emails and mobile phones in one batch, billed only on hits
- **Reverse Email Lookup** — Resolve the person and company behind an email address to enrich existing CRM records
- **Prospect Search** — Query 800M professionals and 50M companies with structured filters (title, seniority, skills, industry, headcount, location) and paginate with offset or cursor
- **Profile Lookup** — Fetch a single person or company profile from an identifier before deciding to spend credits
- **Credit Control** — Check your workspace balance so the agent never over-submits a batch

### How it works

1. Subscribe to this server
2. Grab your **API key** from the [FullEnrich API dashboard](https://app.fullenrich.com/app/api)
3. Ask your agent to build a list, enrich it, and retrieve the results

Enrichment is asynchronous: the agent submits a batch, receives an enrichment ID, and polls (or uses a webhook) for finished records. LinkedIn URLs improve email hit rates by 5-20% and phone hit rates by 10-60%.

### Who is this for?

- **GTM & RevOps engineers** — automate prospect-list building and CRM enrichment without manual tool-hopping
- **Sales development reps** — find deliverable emails and mobile numbers with vendor-breadth accuracy
- **Data teams** — normalize and verify contact records programmatically with per-hit billing


## Available Tools (8)
- **get_enrichment_results**: 164, plus the profile when linkedin_url was provided. While IN_PROGRESS the API errors — wait and retry instead of polling every few seconds.

Fetch the status and enriched records of a bulk job
- **lookup_company**: Provide at least one identifier; domain or professional-network URL/ID give the most reliable match.

Look up a single company and its firmographic profile
- **search_companies**: Synchronous and consumes no credits. Paginate with limit/offset, or the search_after cursor beyond offset 10000.

Search a database of 50M companies with structured filters
- **start_enrichment**: Async: returns an enrichment_id immediately — poll get_enrichment_results no more than once every few minutes (60 calls/min limit shared across all endpoints). A linkedin_url improves hit rates and returns the full contact/company profile too.

Submit contacts for waterfall enrichment across 25+ data vendors
- **start_reverse_lookup**: Async: returns an enrichment_id — retrieve with get_enrichment_results (kind="reverse_email").

Resolve people and companies from email addresses in bulk
- **get_credits**: Use to gate spend before submitting large batches.

Get the current workspace credit balance
- **lookup_person**: Provide at least one identifier — a professional-network URL/ID is the most reliable; a name alone is ambiguous, combine it with a company identifier.

Look up a single professional and their full profile
- **search_people**: Synchronous and consumes no credits. Paginate with limit (max 100) and offset; beyond offset 10000 pass the search_after cursor returned in the previous response.

Search a database of 800M professionals with structured filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FullEnrich** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find 20 heads of sales operations at software companies with 200-1000 employees in the US, then enrich them with work emails."

**🤖 AI Agent:**
> I searched the people database with current_position_titles=Head of Sales Operations, current_company_industries=Software Development, US HQ and headcount 200-1000, and submitted the first 20 contacts with enrich_fields=[contact.work_emails]. The batch returned enrichment_id 2db5ea61-1752-42cf-8ea1-ab1da060cd0a — work emails are ready for 18 of 20 (2 are still in progress).

---

**👤 You:**
> "Who is behind john.snow@acme.com and what's their current company?"

**🤖 AI Agent:**
> I submitted a reverse email lookup for john.snow@acme.com. The resolved profile: John Snow, Head of Sales Operations at Example Inc (example.com, 250 employees, San Francisco). Would you like me to pull the mobile number too?


## ❓ FAQ

**Q: Where do I get my FullEnrich API key?**
Log in to [app.fullenrich.com](https://app.fullenrich.com/app/api) and copy the workspace API key shown on the API dashboard. The key is also the secret used to sign webhooks.

**Q: Why does enrichment return an ID instead of results?**
Enrichment is asynchronous and takes about 30-90 seconds per contact. start_enrichment returns an enrichment_id; retrieve finished records with get_enrichment_results (or set a webhook_url). Poll at most every few minutes — polling shares the same 60 calls/minute budget.

**Q: How does credit billing work?**
Credits are billed only when data is actually found and verified: roughly 1 credit per work email, 3 per personal email and 10 per mobile phone. Use get_credits to check your balance before submitting large batches.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fullenrich](https://vinkius.com/en/ai-agent-connect/fullenrich)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FullEnrich** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fullenrich` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FullEnrich** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fullenrich": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
