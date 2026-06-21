# World Bank Economy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/world-bank-economy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Instantly query GDP, inflation, economic growth, and financial sector indicators from the World Bank. Zero auth required.

## Description
Empower your AI agent with instant access to the World Bank's economic data.

### What you can do
- **GDP Analytics** — Retrieve GDP, GDP per capita, and year-over-year economic growth.
- **Inflation** — Track consumer price changes globally.
- **Interest Rates** — Monitor real interest rates for any country.

### How it works
1. Subscribe to the server.
2. Skip the auth configuration (it's completely open!).
3. Start investigating the global economy.

### Who is this for?
Economists, financial analysts, and market researchers building global macro models.


## Available Tools
- **get_gdp**: Get Gross Domestic Product (GDP) in current US$
- **get_gdp_growth**: Get annual GDP growth percentage
- **get_inflation**: Get inflation rate (consumer prices, annual %)
- **get_economy_indicator**: Get any World Bank economy indicator by its code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **World Bank Economy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the GDP of Brazil compared to Argentina over the last 10 years?"

**🤖 AI Agent:**
> 🌍 **GDP Comparison: Brazil vs Argentina (2014–2024)**

Brazil's GDP stands at approximately $2.1 trillion, while Argentina's hovers around $640 billion. Over the past decade, Brazil has maintained roughly 3× the economic output of Argentina, though both experienced contractions during the pandemic period.

---

**👤 You:**
> "What is the current inflation rate in Turkey?"

**🤖 AI Agent:**
> 🌍 **Inflation: Turkey**

Turkey has experienced extreme inflationary pressure, with consumer prices exceeding 50% annually in recent years — one of the highest rates among G20 economies.

---

**👤 You:**
> "Show me the GDP per capita growth trend for South Korea since 1990."

**🤖 AI Agent:**
> 🌍 **GDP Per Capita: South Korea (1990–2024)**

South Korea's GDP per capita has surged from ~$6,500 in 1990 to over $34,000 today — a remarkable 5× increase reflecting the nation's rapid industrialization and tech-driven economy.


## ❓ FAQ

**Q: How do I get started?**
Our World Bank Open Data servers require absolutely zero authentication. You do not need to register, get an API key, or setup webhooks. Just instantly connect and your AI agent can begin querying decades of global data.

**Q: Can my AI compare the GDP of multiple countries?**
Yes. Your agent can ask for the GDP of Brazil, India, and China over the last 10 years and generate a comprehensive comparative analysis.

**Q: What if I need an obscure financial indicator?**
The server includes an all-access tool where your agent can provide any standard World Bank economic indicator code (like FD.AST.PRVT.GD.ZS) to pull exactly the dataset you need.

**Q: What is the scale of the data I can access?**
You have direct access to 64 years of historical data covering 196+ sovereign states and global regional aggregates, powered directly by the World Bank's robust open data initiatives.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/world-bank-economy](https://vinkius.com/mcp/world-bank-economy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **World Bank Economy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `world-bank-economy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **World Bank Economy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "world-bank-economy": {
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
