# Lusha MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lusha)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Equip your AI agent with direct access to Lusha — find verified B2B contact details, enrich prospect data, and build lead lists without opening the Lusha platform.

## Description
Connect **Lusha** to your AI agent and access verified B2B contact data for your sales prospecting.

### What you can do

- **Contact Enrichment** — Find verified emails, direct dial phone numbers, and social profiles for any prospect.
- **Company Data** — Pull firmographic data including industry, employee count, revenue range, and headquarters location.
- **Prospect Search** — Build targeted prospect lists filtered by job title, seniority, company size, and geography.
- **Bulk Enrichment** — Enrich multiple contacts at once from your existing CRM or lead lists.

### How it works

1. Subscribe to the Lusha integration on the marketplace.
2. Copy your API key from your Lusha dashboard (Settings → API → copy token).
3. Ask your AI agent to find contacts, enrich records, or build prospect lists.

### Who is this for?

- **SDR Teams** — Get direct dials and verified emails instantly for cold outreach campaigns.
- **Sales Teams** — Enrich CRM records before outreach to increase connection and response rates.
- **Recruiters** — Find candidate contact details quickly for direct sourcing.


## Available Tools (6)
- **get_credits**: Get credit balance
- **find_person**: Find person
- **find_company**: Find company
- **bulk_enrich**: Bulk enrich emails
- **find_by_linkedin**: Find by LinkedIn URL
- **search_contacts**: Search contacts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lusha** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the contact details for John Smith, VP Sales at TechCo."

**🤖 AI Agent:**
> Found: John Smith. Email: john.smith@techco.com (verified). Direct dial: +1-555-0147. Mobile: +1-555-0293. LinkedIn: linkedin.com/in/johnsmith-techco. Credits used: 1. Remaining: 149.

---

**👤 You:**
> "Enrich this list of 5 contacts from my CRM."

**🤖 AI Agent:**
> Bulk enrichment complete: 5 contacts processed. 4 found (emails + phone numbers verified), 1 not found (insufficient data). Credits used: 4. Total remaining: 146.

---

**👤 You:**
> "Search for marketing directors at fintech companies in London."

**🤖 AI Agent:**
> Found 28 Marketing Directors at fintech companies in London. Top 3: Emma Clarke (Revolut, verified email + direct dial), David Park (Monzo, verified email), and Sarah Ahmed (Starling Bank, verified email + mobile).


## ❓ FAQ

**Q: How do I get my Lusha API key?**
Log in to your Lusha account at **dashboard.lusha.com**. Click the **Settings** (gear icon) in the left sidebar. Navigate to the **API** section. Your API key is displayed on this page — click **Copy** to copy it. Paste it into the configuration field below. API access is available on Lusha's **Premium** and **Scale** plans.

**Q: Can I find phone numbers and emails for a specific prospect?**
Yes. Provide a person's name and company, and Lusha returns verified business email, personal email, direct dial, mobile number, and LinkedIn profile — all from its database of 100M+ business profiles.

**Q: How many credits does each search consume?**
Each contact enrichment uses 1 credit from your Lusha plan. Credits refresh monthly. Your AI agent reports remaining credits so you always know your usage — no surprises on your bill.

**Q: Is the data GDPR compliant?**
Yes. Lusha is ISO 27701 certified and GDPR/CCPA compliant. All contact data is sourced from publicly available information and community-contributed data with proper consent mechanisms.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lusha](https://vinkius.com/mcp/lusha)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lusha** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lusha` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lusha** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lusha": {
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
