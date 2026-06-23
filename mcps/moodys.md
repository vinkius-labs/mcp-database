# Moody's MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moodys)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Credit ratings and risk analysis — access issuer ratings, issue details, and rating actions via Moody's.

## Description
Empower your AI agents with world-class financial intelligence. The **Moody's Ratings API** integration provides programmatic access to credit ratings, research, and risk metrics for thousands of issuers and financial instruments.

### What you can do

- **Issuer Monitoring** — Retrieve and track credit ratings and outlooks for global entities
- **Security Analysis** — Access detailed ratings and metadata for specific financial issues (CUSIP/ISIN)
- **Event Tracking** — Stay updated on the latest rating actions, upgrades, and downgrades
- **Market Research** — Search for entities and explore market segments covered by Moody's

### How it works

1. Subscribe to this server
2. Enter your **Moody's API Key** from the API Hub
3. Start querying credit intelligence directly from your favorite MCP client


## Available Tools (8)
- **get_issue_details**: Get detailed info for an issue
- **get_issuer_details**: Get detailed info for an issuer
- **get_market_segments**: List market segments
- **get_rating_reference**: Get rating scale reference
- **list_issue_ratings**: List credit ratings for specific issues
- **list_issuer_ratings**: List credit ratings for issuers
- **list_rating_actions**: List recent rating actions
- **search_entities**: Search for issuers or organizations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moody's** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current Moody's rating for 'Apple Inc.'?"

**🤖 AI Agent:**
> Searching for Apple Inc... I've found the issuer details. The current rating is 'Aa1' with a 'Stable' outlook.

---

**👤 You:**
> "Show recent rating actions in the banking sector."

**🤖 AI Agent:**
> Retrieving recent actions... There were 5 rating changes in the banking sector this week, including 2 upgrades and 1 outlook revision.


## ❓ FAQ

**Q: How do I get a Moody's API Key?**
Register at developer.moodys.com, create a project, and generate an API key in your account settings.

**Q: Does this cover ESG or Climate ratings?**
This server focus on the core Credit Ratings API. ESG and Climate data may require separate API products and scopes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moodys](https://vinkius.com/mcp/moodys)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moody's** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moodys` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moody's** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moodys": {
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
