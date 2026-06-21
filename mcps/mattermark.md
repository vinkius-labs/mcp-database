# Mattermark MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mattermark)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Startup and venture capital data via Mattermark — search companies, investors, and funding rounds.

## Description
Connect your **Mattermark** account to any AI agent and access deep insights into the startup ecosystem through natural conversation.

### What you can do

- **Company Research** — Search for startups, fetch detailed metadata, and monitor funding history
- **Investor Intelligence** — List venture firms and inspect their portfolios and profiles
- **Funding Rounds** — Query specific investment rounds and their details
- **Competitive Analysis** — Find similar companies and track employee growth trends

### How it works

1. Subscribe to this server
2. Enter your Mattermark API Key
3. Start querying startup and VC data from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_company_details**: Get details for a specific company
- **get_company_employees**: Get employee data for a company
- **get_company_funding_rounds**: Get funding history for a company
- **get_company_news**: Get news for a specific company
- **get_funding_round_details**: Get details for a funding round
- **get_investor_details**: Get details for an investor
- **list_investors**: List venture capital investors
- **list_similar_companies**: Find similar companies
- **search_companies**: Search for companies
- **search_funding_rounds**: Search for funding rounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mattermark** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for companies in the 'Fintech' sector in New York."

**🤖 AI Agent:**
> Fetching companies... I found several fintech startups in New York, including 'Better.com' and 'Plaid'.

---

**👤 You:**
> "Get funding history for company ID 123."

**🤖 AI Agent:**
> Retrieving funding rounds... Company 123 has raised a total of $50M across 3 rounds (Seed, Series A, Series B).

---

**👤 You:**
> "List similar companies to 'Stripe'."

**🤖 AI Agent:**
> Searching for similar companies... I found 'Adyen', 'PayPal', and 'Square' as related entities.


## ❓ FAQ

**Q: How do I find my Mattermark API Key?**
Log in to Mattermark and go to your Account Settings to find and copy your API Key.

**Q: What kind of company data can I access?**
You can access company metadata, funding rounds, news, employee counts, and location info.

**Q: Is my API Key secure?**
Yes. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mattermark](https://vinkius.com/mcp/mattermark)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mattermark** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mattermark` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mattermark** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mattermark": {
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
