# Bureau of Labor Statistics Full — The Mega Server MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bureau-of-labor-statistics-full-the-mega-server-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

The ultimate BLS Mega-Server: Access all 6 major datasets including CPI (Inflation), CES (Jobs), CPS (Unemployment), JOLTS (Turnover), LAUS (Local metrics), and OEWS (Wages by Profession).

## Description
The **ultimate U.S. BLS Mega-Server** gives your agent omnipotent access to the American labor market and economy.

### Included Datasets
- 📈 **Prices** — CPI-U, PPI, Inflation historic tracking
- 💼 **Jobs** — Nonfarm payrolls, hourly earnings
- 📉 **Labor Force** — National unemployment, participation rates
- 🔄 **JOLTS** — The Great Resignation tracking, Quits vs Hires
- 📍 **Local Area** — State and County level unemployment arrays
- 💵 **Occupational Wages** — Hyper-specific wages per physical location per job title

### How it works
1. Sign up for a free BLS Developer API Key
2. Configure your agent
3. Unleash macroeconomic insights across 20-year deep datasets

### Who is this for?
- **Enterprise AI Systems** — Omniscient macro analysis
- **Research Institutions** — Boundless array processing
- **Hedge Funds** — Full economic picture modeling


## Available Tools
- **query_bls**: Use this instead of specific endpoints if you intimately know the underlying numerical code. Up to 50 concurrent lookbacks allowed.

Generic BLS v2 api timeseries query. Requires explicit BLS Series IDs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bureau of Labor Statistics Full — The Mega Server** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me the total economic wrap-up: Inflation, Nonfarm payrolls, and Unemployment rate for the last month."

**🤖 AI Agent:**
> 📊 **Macroeconomic Indicator Suite**

1. **Inflation (CPI-U)**: +0.3% MoM (3.4% YoY)
2. **Jobs (Nonfarm)**: +216,000 jobs added
3. **Unemployment (CPS)**: 3.7% (unchanged)

These combined BLS metrics indicate a resilient labor market supporting a soft landing for inflation.

---

**👤 You:**
> "Cross-reference finding jobs in Software Engineering with the average pay utilizing OEWS and JOLTS."

**🤖 AI Agent:**
> 💵 **Cross-Analysis: Tech Sector Demand**

Using JOLTS, the 'Information' sector shows 105,000 open roles. Cross-referencing OEWS (Code 15-1252), the median wage for Software Developers sits at **$132,270** annually. The combined metrics show extremely high retention and premium compensation remaining steady.

---

**👤 You:**
> "Compare the Local Area Unemployment in Texas vs California down to the exact points."

**🤖 AI Agent:**
> 📍 **LAUS Comparison: TX vs CA**

- **Texas**: 3.9% Unemployment (Stable)
- **California**: 5.1% Unemployment (Rising)

Texas currently maintains a stark advantage in labor absorption rates compared to the tightening markets in California metros.


## ❓ FAQ

**Q: Why merge them all into a Mega-Server?**
Economics isn't isolated. An AI needs to simultaneously access Wage data (OEWS), Jobs data (CES), and Inflation data (CPI) to provide real context. The Mega-Server allows a single agent to paint the entire U.S. macroeconomic picture without missing puzzle pieces.

**Q: Does this require multiple API keys?**
No, a single free Developer Registration Key from the Bureau of Labor Statistics works across all of these datasets interchangeably. You paste it once, and your AI accesses the whole suite.

**Q: What is LAUS and OEWS?**
LAUS is Local Area Unemployment — letting your AI zoom down to county-level employment metrics. OEWS is Occupational Wages — letting your AI see exactly what a specific job title (e.g., Dental Hygienist) makes in a specific state.

**Q: Is the BLS Mega-Server safe to auto-run?**
Yes. The BLS API v2 processes payloads of up to 50 complex series across 20-year lookbacks in single POST requests. It is designed precisely for heavy, automated, multi-dataset lifting without timing out your agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bureau-of-labor-statistics-full-the-mega-server-1](https://vinkius.com/mcp/bureau-of-labor-statistics-full-the-mega-server-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bureau of Labor Statistics Full — The Mega Server** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bureau-of-labor-statistics-full-the-mega-server-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bureau of Labor Statistics Full — The Mega Server** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bureau-of-labor-statistics-full-the-mega-server-1": {
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
