# Tieback vs Standalone Economics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tieback-vs-standalone-economics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [oil-and-gas](../categories/oil-and-gas.md)

Compare the financial viability of tieback vs standalone offshore developments.

## Description
This MCP server provides specialized economic decision-support tools for offshore oil and gas development. It allows users to evaluate the trade-offs between connecting a new field to existing infrastructure (tieback) or building a dedicated facility (standalone). The server includes tools to `compare_development_options` by calculating Net Present Value (NPV), `calculate_breakeven_distance` to find the critical distance where development strategies shift, `validate_host_capacity` to ensure production profiles fit within host constraints, and `estimate_operational_costs` to model lifecycle OPEX including host tariffs.


## Available Tools (4)
- **validate_host_capacity**: Verifies if tieback is physically feasible given host capacity
- **calculate_breakeven_distance**: Calculates the distance where tieback becomes less economical than standalone
- **compare_development_options**: Compares NPV for tieback vs standalone development
- **estimate_operational_costs**: Calculates total lifecycle OPEX for both scenarios


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tieback vs Standalone Economics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare the NPV for a field with 100M barrels, 20km distance, a production profile of {"annualRates": [10, 10, 5]}, standalone CAPEX of 500, tieback CAPEX of 100, tariff of 2, capacity of 15, and 10% discount rate."

**🤖 AI Agent:**
> The preferred option is the tieback development with an NPV of 450.2 million, compared to the standalone NPV of 380.5 million.

---

**👤 You:**
> "Is a tieback feasible for a production profile of {"annualRates": [20, 15, 10]} with a host capacity limit of 18?"

**🤖 AI Agent:**
> No, the tieback is not feasible because the peak production in year 1 (20) exceeds the host capacity limit of 18.

---

**👤 You:**
> "What is the break-even distance for a field with 50M barrels, standalone CAPEX of 400, tieback CAPEX per km of 5, tariff of 1, capacity of 10, and 8% discount rate?"

**🤖 AI Agent:**
> The break-even distance is 35.4 km. Beyond this distance, a standalone facility becomes the more economical choice.


## ❓ FAQ

**Q: How does the tool handle host capacity constraints?**
The `validate_host_capacity` tool checks the production profile against the host limit. If any annual production exceeds the limit, the tieback is flagged as infeasible.

**Q: What is the break-even distance?**
It is the distance where the cost of the tieback pipeline equals the cost of a standalone facility, which can be found using `calculate_breakeven_distance`.

**Q: Does the NPV calculation include host tariffs?**
Yes, when using `compare_development_options`, the tieback NPV accounts for the host tariff per barrel produced.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tieback-vs-standalone-economics](https://vinkius.com/en/ai-agent-connect/tieback-vs-standalone-economics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tieback vs Standalone Economics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tieback-vs-standalone-economics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tieback vs Standalone Economics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tieback-vs-standalone-economics": {
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
