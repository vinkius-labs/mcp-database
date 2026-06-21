# Otreeba Cannabis API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/otreeba-cannabis-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Access cannabis strain data, lab results, and brand info via Otreeba API.

## Description
Connect **Otreeba** to any AI agent and access open, verified cannabis data -- search strains, get lab results (THC, CBD, terpenes), and explore cannabis brands through natural conversation.

### What you can do
- **Strain Search** -- Find cannabis strains by name, effects, or keywords
- **Lab Data** -- Retrieve cannabinoid and terpene profiles for flower and oils
- **Brand Directory** -- List and inspect cannabis producers and brands

### How it works
1. Subscribe to this server
2. Enter your Otreeba API Token
3. Start exploring cannabis data from Claude, Cursor, or any MCP-compatible client

Otreeba provides an open, transparent database of cannabis products and lab testing for consumers and industry professionals.

### Who is this for?
- **Cannabis Consumers** -- Verify THC/CBD levels and terpene profiles before purchasing
- **Budtenders & Staff** -- Quickly look up strain effects and lineage to assist customers
- **Industry Analysts** -- Access open data for market research and product analysis


## Available Tools
- **get_flower_lab_data**: ) and terpene data for a specific strain.

Get lab test results for cannabis flower
- **get_brand**: Get details for a specific cannabis brand
- **get_strain**: Get full details for a specific cannabis strain
- **list_brands**: List all cannabis brands available in Otreeba
- **get_oil_lab_data**: Get lab test results for cannabis oil/extracts
- **search_strains**: Use this to discover available strains in the Otreeba database.

Search for cannabis strains by name or keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Otreeba Cannabis API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for Indica strains that help with sleep."

**🤖 AI Agent:**
> Found 5 strains: 1. Granddaddy Purple. 2. Northern Lights. 3. Purple Kush.

---

**👤 You:**
> "Get the lab data for Blue Dream flower."

**🤖 AI Agent:**
> Lab Data: THC: 18.5%, CBD: 0.1%. Terpenes: Myrcene, Pinene, Caryophyllene.

---

**👤 You:**
> "List all cannabis brands in the database."

**🤖 AI Agent:**
> Found 15 brands: 1. Green Cultur. 2. Oasis. 3. Curo. 4. Bloom.


## ❓ FAQ

**Q: How do I get my Otreeba API Token?**
Go to the Otreeba website, create an account or log in, and find your API credentials in the developer or account settings section.

**Q: Does it include lab test results for THC and CBD?**
Yes! The get_flower_lab_data and get_oil_lab_data tools return exact percentages for cannabinoids including THC, CBD, and full terpene profiles.

**Q: Can I search for specific strain effects?**
Yes, the search_strains tool allows you to search by keywords including common effects like 'relaxing', 'energetic', or 'focus'.

**Q: Can I find the seed company or lineage for a strain?**
Yes! Use the search_strains tool to find seed company and lineage information for specific strains in the database.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/otreeba-cannabis-api](https://vinkius.com/mcp/otreeba-cannabis-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Otreeba Cannabis API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `otreeba-cannabis-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Otreeba Cannabis API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "otreeba-cannabis-api": {
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
