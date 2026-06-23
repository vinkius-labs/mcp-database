# World Bank Labor & Trade MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/world-bank-labor-trade)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Analyze global unemployment, labor forces, trade balances (imports/exports), and FDI directly from the World Bank API.

## Description
Leverage the World Bank API to power agentic research into international trade and labor markets.

### What you can do
- **Labor Markets** — Check national unemployment rates and total labor force sizes.
- **International Trade** — Analyze a nation's reliance on exports and imports.
- **Foreign Investment** — Audit Foreign Direct Investment (FDI) inflows across borders.

### How it works
1. Simply subscribe to the server.
2. Your agent automatically has access since it requires no API keys.
3. Make your agent trade-fluent.

### Who is this for?
Supply chain analysts, trade researchers, HR strategists, and international business consultants.


## Available Tools (5)
- **get_unemployment_rate**: Get unemployment total (% of labor force)
- **get_labor_force**: Get total labor force
- **get_exports**: Get exports of goods/services (% of GDP)
- **get_fdi**: Get Foreign Direct Investment, net inflows (% of GDP)
- **get_labor_trade_indicator**: Get any World Bank labor/trade indicator by code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **World Bank Labor & Trade** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How heavily does Germany rely on exports compared to the UK?"

**🤖 AI Agent:**
> 🌍 **Export Dependence: Germany vs UK**

Germany's exports represent approximately 47% of GDP, making it one of the most export-driven major economies. The UK's exports sit around 31% of GDP, reflecting its stronger domestic services orientation.

---

**👤 You:**
> "What is the youth unemployment rate in Spain versus France?"

**🤖 AI Agent:**
> 🌍 **Youth Unemployment: Spain vs France**

Spain historically faces some of Europe's highest youth unemployment, hovering around 28%, while France's rate sits closer to 17%. Both remain well above the EU average.

---

**👤 You:**
> "Which emerging markets attract the most foreign direct investment?"

**🤖 AI Agent:**
> 🌍 **FDI Leaders: Emerging Markets**

Vietnam, India, and Brazil consistently attract the highest FDI inflows among emerging markets, driven by favorable demographics, growing consumer markets, and strategic government incentives.


## ❓ FAQ

**Q: How do I get started?**
Our World Bank Open Data servers require absolutely zero authentication. You do not need to register, get an API key, or setup webhooks. Just instantly connect and your AI agent can begin querying decades of global data.

**Q: Can it show me the total size of a competitive workforce?**
Yes! Your agent can pull the total labor force number to help multi-national corporations decide on global expansion targets and office placements.

**Q: Can my AI analyze foreign direct investment (FDI)?**
Precisely. The agent can pull 'FDI net inflows as % of GDP' to measure how effectively a nation attracts international capital.

**Q: What is the scale of the data I can access?**
You have direct access to 64 years of historical data covering 196+ sovereign states and global regional aggregates, powered directly by the World Bank's robust open data initiatives.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/world-bank-labor-trade](https://vinkius.com/mcp/world-bank-labor-trade)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **World Bank Labor & Trade** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `world-bank-labor-trade` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **World Bank Labor & Trade** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "world-bank-labor-trade": {
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
