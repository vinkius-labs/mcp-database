# EIA Energy Outlook — Forecasts & Projections MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eia-energy-outlook-forecasts-projections)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Official U.S. energy forecasts: the Short-Term Energy Outlook (18-month price and supply projections), Annual Energy Outlook (30-year U.S. projections), International Energy Outlook (world projections), and country-level global energy data.

## Description
Forward-looking energy intelligence from the world's most respected energy agency.

### What you can do
- **STEO** — Short-Term Energy Outlook: 18-month price, production, and consumption projections (updated monthly)
- **AEO** — Annual Energy Outlook: 30-year U.S. energy projections with reference/side cases
- **IEO** — International Energy Outlook: world energy projections by region and fuel
- **International Data** — Country-level production, consumption, trade, and emissions

### Who is this for?
Energy strategists, government planners, investment analysts, climate modelers, and anyone who needs the official U.S. government view on where energy markets are heading.


## Available Tools
- **get_short_term_outlook**: Published monthly by EIA. Data range: 1974 to 2027.

Get STEO: 18-month U.S. energy price and supply projections
- **get_annual_outlook**: S. energy production, consumption, prices, and emissions using the National Energy Modeling System (NEMS). Includes reference case and side cases.

Get AEO: 30-year U.S. energy projections
- **get_international_outlook**: Covers global production, consumption, and emissions by region and fuel.

Get IEO: international energy projections
- **get_international_data**: Get country-level energy production, consumption, and emissions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EIA Energy Outlook — Forecasts & Projections** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What does EIA forecast for oil prices next year?"

**🤖 AI Agent:**
> 🔮 **STEO — Oil Price Forecast**

Brent crude:
- Q1 2025: $82/bbl
- Q2 2025: $79/bbl
- Q3 2025: $77/bbl
- Q4 2025: $75/bbl
- 2025 avg: $78/bbl

EIA expects gradual price decline as non-OPEC production grows faster than demand.

---

**👤 You:**
> "How does EIA project U.S. energy mix in 2050?"

**🤖 AI Agent:**
> 🌍 **AEO 2050 — U.S. Energy Mix (Reference Case)**

Electricity generation:
- Renewables: 44% (from 22% today)
- Natural Gas: 34% (from 43%)
- Nuclear: 12% (from 19%)
- Coal: 6% (from 16%)
- Other: 4%

Solar and wind drive the massive renewable growth.

---

**👤 You:**
> "Compare energy consumption between China and India"

**🤖 AI Agent:**
> 🌏 **China vs India — Energy Consumption**

| Metric | China | India |
|--------|-------|-------|
| Total (Quad BTU) | 159.4 | 35.2 |
| Per capita | 113 MMBTU | 25 MMBTU |
| Coal share | 56% | 55% |
| Oil share | 20% | 27% |
| Renewables | 15% | 10% |

China consumes 4.5× more energy than India.


## ❓ FAQ

**Q: How far ahead does EIA forecast?**
Three horizons: **STEO** covers 18 months ahead (updated monthly). **AEO** projects 30 years for the U.S. **IEO** projects 25+ years for the global market. Each uses different models: STEO for short-term, NEMS for AEO, WEPS for IEO.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eia-energy-outlook-forecasts-projections](https://vinkius.com/mcp/eia-energy-outlook-forecasts-projections)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EIA Energy Outlook — Forecasts & Projections** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `eia-energy-outlook-forecasts-projections` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EIA Energy Outlook — Forecasts & Projections** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eia-energy-outlook-forecasts-projections": {
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
