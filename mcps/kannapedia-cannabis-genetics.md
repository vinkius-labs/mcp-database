# Kannapedia Cannabis Genetics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kannapedia-cannabis-genetics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search cannabis strains, terpenes, and effects via Kannapedia.

## Description
Connect **Kannapedia** to any AI agent and access a comprehensive cannabis genetics database -- search strains by name, filter by dominant terpenes, or find genetics based on specific effects through natural conversation.

### What you can do
- **Strain Search** -- Find genetics by name or keyword
- **Terpene Profiles** -- Search strains by dominant terpenes like Myrcene or Limonene
- **Effect Filtering** -- Discover strains associated with specific effects like Sleep or Focus
- **Strain Details** -- Get full lineage and description data

### How it works
1. Subscribe to this server
2. Enter your Kannapedia API Key
3. Start exploring cannabis genetics from Claude, Cursor, or any MCP-compatible client

Kannapedia is a specialized resource for cannabis genetics, providing structured data on strains, terpenes, and reported effects for researchers and consumers.

### Who is this for?
- **Consumers** -- Find strains with specific terpene profiles or effects
- **Budtenders** -- Quickly recommend genetics based on customer preferences
- **Researchers** -- Access structured genetics data for studies and analysis


## Available Tools (4)
- **search_by_effect**: g., Relaxed, Energetic, Sleepy).

Search strains by reported effect
- **get_strain_detail**: Get detailed information for a specific strain
- **search_genetics**: Use this to discover specific genetics in the Kannapedia database.

Search cannabis strains by name or keyword
- **search_by_terpene**: g., Myrcene, Limonene).

Search strains by dominant terpene


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kannapedia Cannabis Genetics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for strains high in Limonene."

**🤖 AI Agent:**
> Found 3 strains: 1. Super Lemon Haze. 2. Banana Kush. 3. Do-Si-Dos.

---

**👤 You:**
> "Show me details for OG Kush."

**🤖 AI Agent:**
> OG Kush (Hybrid): Lineage: Chemdawg x Lemon Thai x Pakistani Kush. Effects: Euphoric, Happy, Relaxed.

---

**👤 You:**
> "Find strains that help with Sleep."

**🤖 AI Agent:**
> Found 5 strains: 1. Granddaddy Purple. 2. Northern Lights. 3. 9 Pound Hammer.


## ❓ FAQ

**Q: How do I get my Kannapedia API Key?**
Sign up on the Kannapedia website, navigate to your account settings, and generate a new API key for developer access.

**Q: Can I search for specific terpenes?**
Yes, the search_by_terpene tool allows you to find strains known for dominant terpenes like Myrcene, Limonene, or Caryophyllene.

**Q: Does it include lineage and parentage?**
Yes, the get_strain_detail tool provides full lineage data, including parent strains and genetic background for each entry.

**Q: Can I filter strains by their reported effects?**
Yes! Use the search_by_effect tool to discover strains associated with specific effects such as Sleep, Focus, or Relaxation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kannapedia-cannabis-genetics](https://vinkius.com/mcp/kannapedia-cannabis-genetics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kannapedia Cannabis Genetics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kannapedia-cannabis-genetics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kannapedia Cannabis Genetics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kannapedia-cannabis-genetics": {
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
