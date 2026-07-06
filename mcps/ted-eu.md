# TED EU MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ted-eu)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Search EU public procurement tenders via TED — find contracts by country, sector, or value range from any AI agent.

## Description
Connect **TED (Tenders Electronic Daily)** to any AI agent and search EU public procurement opportunities through natural conversation instead of navigating complex procurement portals.

### What you can do

- **Full-Text Search** — Search across all TED procurement notices using keywords like "software development" or "medical equipment"
- **Country Filtering** — Find active tenders from any of the 27 EU member states using ISO country codes
- **CPV Classification** — Search by Common Procurement Vocabulary codes to target specific industry sectors
- **Value Range Search** — Filter tenders by contract value in EUR to match your company size and capacity
- **Recent Opportunities** — Monitor newly published tenders from the last 7 days to stay ahead of deadlines
- **Notice Details** — Retrieve full procurement details including lots, award criteria, timelines, and contracting authority contacts

### How it works

1. Subscribe to this server
2. Optionally enter a TED API Key for higher rate limits (anonymous access works for basic searches)
3. Start finding procurement opportunities from Claude, Cursor, or any MCP-compatible client

TED is the official publication platform of the European Union for public procurement notices, publishing over 700,000 contract opportunities annually.

### Who is this for?

- **Business Development Teams** — discover relevant government contracts across Europe without manually browsing TED
- **Procurement Consultants** — quickly assess market opportunities for clients in specific sectors or countries
- **Public Affairs Analysts** — monitor procurement trends and spending patterns across EU member states


## Available Tools (6)
- **search_tenders**: Returns title, country, value, deadline, and contracting authority. Covers all 27 EU member states.

Search EU public tenders
- **search_by_country**: Use ISO country codes: DE, FR, ES, IT, PT, NL, etc.

Search tenders by country
- **search_by_cpv**: CPV codes classify EU contracts by sector: 72000000 (IT), 45000000 (Construction), 33000000 (Medical).

Search tenders by CPV code
- **search_by_value**: Useful for finding contracts matching your company size.

Search tenders by contract value
- **list_recent_tenders**: Default is 7 days. Use to monitor new opportunities.

List recently published tenders
- **get_tender**: Includes description, lots, award criteria, timelines, and contracting authority contact.

Get tender notice details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TED EU** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find recent tenders for software development in France."

**🤖 AI Agent:**
> Found 8 active tenders matching 'software development' in France:
1. FR-2025/S-089-234567 — "Cloud migration platform" — Ministry of Finance — €2.4M — Deadline: April 28
2. FR-2025/S-091-345678 — "Healthcare records system" — CHU Bordeaux — €890K — Deadline: May 5
3. FR-2025/S-092-456789 — "Transport management SaaS" — SNCF — €1.7M — Deadline: May 12
Showing 3 of 8. Want me to get full details on any of these?

---

**👤 You:**
> "Show me construction tenders worth over 5 million euros."

**🤖 AI Agent:**
> Found 15 tenders in CPV 45000000 (Construction) above €5M:
1. DE-2025/S-087-123456 — "Highway A3 expansion Cologne-Frankfurt" — €47M — Deadline: April 20
2. ES-2025/S-088-234567 — "Hospital Universitario renovation" — €12.3M — Deadline: May 1
3. IT-2025/S-090-345678 — "Metro Line C extension Rome" — €89M — Deadline: May 15
Showing 3 of 15. Filter by country or narrow the value range?

---

**👤 You:**
> "What new tenders were published this week?"

**🤖 AI Agent:**
> 342 new tenders published in the last 7 days. Top sectors:
• IT Services (CPV 72): 48 notices
• Construction (CPV 45): 67 notices
• Medical Equipment (CPV 33): 31 notices
• Transport (CPV 60): 22 notices
Top countries: Germany (71), France (54), Spain (38), Italy (42). Want me to drill into a specific sector or country?


## ❓ FAQ

**Q: Do I need an API key to use TED?**
No! The TED Search API allows anonymous access for basic queries. An API key only increases your rate limits for high-volume usage. You can start searching tenders immediately without any credentials. If you need higher throughput, get a free key at developer.ted.europa.eu.

**Q: How can I find IT contracts over 500K EUR in Germany?**
Combine tools: use `search_by_cpv` with code 72000000 (IT services) or `search_by_country` with code DE, then ask your agent to filter by value. Or use `search_by_value` with min_value 500000 and max_value 10000000. Your agent cross-references the results to show only German IT contracts above your threshold.

**Q: Is TED data limited to EU countries only?**
TED primarily covers the 27 EU member states, but it also includes notices from EEA countries (Norway, Iceland, Liechtenstein), EU candidate countries, and some international organizations. All tools return data across this full scope. The `search_by_country` tool supports ISO codes for all covered territories.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ted-eu](https://vinkius.com/mcp/ted-eu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TED EU** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ted-eu` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TED EU** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ted-eu": {
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
