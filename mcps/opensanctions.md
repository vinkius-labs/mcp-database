# OpenSanctions MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opensanctions)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Screen persons and companies against global sanctions lists and PEP databases for KYC/AML compliance.

## Description
Connect to **OpenSanctions** and access the world's largest open sanctions and PEP screening database through natural conversation — no API key needed for non-commercial use.

### What you can do

- **Entity Search** — Search for sanctioned persons, companies and vessels by name
- **Sanctions Screening** — Screen names against global sanctions lists (OFAC, EU, UN, UK HMT)
- **PEP Screening** — Screen persons against Politically Exposed Persons databases
- **Entity Details** — Get full entity info including aliases, dates of birth, nationalities and addresses
- **Vessel Search** — Search sanctioned vessels by name or IMO number
- **Dataset Browser** — Browse all available sanctions datasets worldwide

### How it works

1. Subscribe to this server
2. No API key needed for non-commercial use
3. Start screening against sanctions lists from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Compliance Officers** — screen clients and partners against global sanctions lists
- **Financial Institutions** — perform KYC/AML checks on customers and transactions
- **Researchers** — explore sanctions data, PEP databases and entity relationships


## Available Tools (8)
- **get_entity**: Returns full entity details including names, aliases, dates of birth, nationalities, addresses, sanctions details, related entities and source datasets.

Get detailed info for a specific entity by ID
- **match_pep**: Returns match scores, matched entities, political positions and source datasets. Useful for KYC/AML compliance checks.

Screen a name against Politically Exposed Persons (PEP) lists
- **match_sanctions**: Uses fuzzy matching to find potential matches. Returns match scores, matched entities and sanction details. Use threshold parameter (0.0-1.0) to adjust sensitivity. Default 0.85.

Screen a name against global sanctions lists
- **search_company**: Returns company names, registration numbers, jurisdictions, addresses and sanctions status.

Search for companies in the sanctions database
- **search_entities**: Supports free-text search with fuzzy matching. Returns entity names, types (Person, Company, Vessel), countries and dataset sources. Use schema parameter to filter by entity type (Person, Company, Vessel, etc.).

Search sanctions and PEP entities by name
- **search_person**: Returns person names, aliases, dates of birth, nationalities, countries and sanctions status.

Search for persons in the sanctions database
- **search_vessel**: Returns vessel names, IMO numbers, flags, owners and sanctions status.

Search for vessels (ships) in the sanctions database
- **get_datasets**: Returns dataset names, descriptions, publisher info and entity counts.

Get list of all sanctions datasets available


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenSanctions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Screen 'Vladimir Putin' against sanctions lists."

**🤖 AI Agent:**
> Found multiple matches for Vladimir Putin in OFAC, EU and UK sanctions lists. Includes aliases, dates of birth, nationalities and sanctions details.

---

**👤 You:**
> "Search for companies sanctioned in Russia."

**🤖 AI Agent:**
> Found 50+ sanctioned companies with Russian connections. Includes Gazprom, Rosneft, Sberbank and many others across OFAC, EU and UK sanctions lists.

---

**👤 You:**
> "What sanctions datasets are available?"

**🤖 AI Agent:**
> Available datasets: US OFAC (9,000+ entities), EU Consolidated List (6,000+), UN Security Council (700+), UK HMT (3,000+), and 40+ more global sanctions regimes.


## ❓ FAQ

**Q: Do I need an API key?**
No! OpenSanctions is completely free for non-commercial use. No authentication required.

**Q: What sanctions lists are included?**
OpenSanctions aggregates data from OFAC (US), EU Consolidated List, UN Security Council, UK HMT, and many other global sanctions regimes.

**Q: How accurate is the name matching?**
The API uses fuzzy matching with configurable thresholds (0.0-1.0). Default threshold of 0.85 balances accuracy and recall for most use cases.

**Q: Can I screen companies, not just individuals?**
Yes! Use search_company to find sanctioned companies, or use the general search with schema='Company' filter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opensanctions](https://vinkius.com/mcp/opensanctions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenSanctions** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `opensanctions` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenSanctions** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opensanctions": {
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
