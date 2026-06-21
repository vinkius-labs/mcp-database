# Country Data Resolver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/country-data-resolver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Resolve ISO country codes to full names, alpha-3, and numeric codes in 4 languages. Essential for CRM and international data.

## Description
When a CRM agent processes international contacts, it cannot guess that 'MK' is North Macedonia or that 'TL' is Timor-Leste. This MCP resolves any ISO 3166-1 alpha-2 code to its full name in English, Portuguese, Spanish, or French.

### The Superpowers

- **249 Countries:** Full ISO 3166-1 database with alpha-2, alpha-3, and numeric codes.
- **4 Languages:** Country names in EN, PT, ES, and FR for multilingual CRM workflows.


## Available Tools
- **resolve_country**: Pass the alpha-2 code (e.g. "BR", "DE", "JP") and optionally a language for the name (en, pt, es, fr). Never guess country names for obscure codes.

Resolves ISO country codes to full country names in 4 languages, plus alpha-3 and numeric codes. Essential for CRM and Martech agents handling international data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Country Data Resolver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the full name for country code BR in Portuguese?"

**🤖 AI Agent:**
> Country: Brasil (alpha-3: BRA, numeric: 076)

---

**👤 You:**
> "Resolve the country code MK to its full name."

**🤖 AI Agent:**
> Country: North Macedonia (alpha-3: MKD, numeric: 807)

---

**👤 You:**
> "Get all ISO codes for Japan."

**🤖 AI Agent:**
> Country: Japan (alpha-2: JP, alpha-3: JPN, numeric: 392)


## ❓ FAQ

**Q: How many countries are supported?**
All 249 countries and territories in the ISO 3166-1 standard, including overseas territories and special regions.

**Q: What languages are available for country names?**
English (en), Portuguese (pt), Spanish (es), and French (fr). The engine defaults to English if the requested language is not available.

**Q: Does it validate country codes?**
Yes. If you pass an invalid code like 'XX', the engine returns a clear error instead of guessing. This prevents data corruption in CRM systems.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/country-data-resolver](https://vinkius.com/mcp/country-data-resolver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Country Data Resolver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `country-data-resolver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Country Data Resolver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "country-data-resolver": {
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
