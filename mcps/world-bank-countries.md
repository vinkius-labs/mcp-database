# World Bank Countries MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/world-bank-countries)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

The definitive geographic metadata API for resolving country ISO codes, geographic regions, and global income/lending classifications.

## Description
Provide your AI agent with the World Bank's master taxonomy of geography to build deeply accurate filtering and mapping tools.

### What you can do
- **Country List** — Rapidly retrieve massive lists of countries, their exact ISO standards, and capital cities.
- **Regions & Lending** — Identify macroscopic regional blocks or a country's classification logic.
- **Income Taxonomies** — Perfect standard groupings (e.g. searching 'HIC' High Income Countries).

### How it works
1. Simply subscribe.
2. Skip the API configuration step—it works immediately.
3. Make your agent geographically fluent.

### Who is this for?
Data engineers, global cartography apps, economic planners, and macro analysts.


## Available Tools (3)
- **list_countries**: List World Bank countries
- **search_regions**: List World Bank geographic regions
- **search_income_levels**: g., HIC, LIC).

List World Bank income levels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **World Bank Countries** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all high-income countries in East Asia."

**🤖 AI Agent:**
> 🌍 **High-Income Countries: East Asia**

Japan (JPN), South Korea (KOR), Singapore (SGP), Hong Kong SAR (HKG), and Macao SAR (MAC) are classified as High Income Countries (HIC) in the East Asia & Pacific region by the World Bank.

---

**👤 You:**
> "What are the World Bank geographic regions?"

**🤖 AI Agent:**
> 🌍 **World Bank Regions**

1. East Asia & Pacific
2. Europe & Central Asia
3. Latin America & Caribbean
4. Middle East & North Africa
5. North America
6. South Asia
7. Sub-Saharan Africa

---

**👤 You:**
> "Show me the income level classification for all South American countries."

**🤖 AI Agent:**
> 🌍 **Income Levels: South America**

Upper-Middle Income: Brazil, Colombia, Peru, Argentina, Ecuador, Paraguay. High Income: Chile, Uruguay. Lower-Middle Income: Bolivia. The classification is based on GNI per capita thresholds set by the World Bank annually.


## ❓ FAQ

**Q: How do I get started?**
Our World Bank Open Data servers require absolutely zero authentication. You do not need to register, get an API key, or setup webhooks. Just instantly connect and your AI agent can begin querying decades of global data.

**Q: Can it map complex regions without hardcoding ISO values?**
Yes! Your agent queries the `/country` endpoint to dynamically resolve geographic mappings in real time, no static lists required.

**Q: Does it classify nations into income tiers?**
Yes. Use the income-level resolution tools so your AI can immediately segregate advanced economies from developing nations based on precise World Bank thresholds.

**Q: What is the scale of the data I can access?**
You have direct access to 64 years of historical data covering 196+ sovereign states and global regional aggregates, powered directly by the World Bank's robust open data initiatives.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/world-bank-countries](https://vinkius.com/mcp/world-bank-countries)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **World Bank Countries** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `world-bank-countries` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **World Bank Countries** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "world-bank-countries": {
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
