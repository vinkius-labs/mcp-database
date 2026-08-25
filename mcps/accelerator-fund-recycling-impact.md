# Accelerator Fund Recycling Impact MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-fund-recycling-impact)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantify the financial effects of recycling realized gains into new fund deployments.

## Description
This MCP server provides analytical tools for venture capital managers to model the impact of recycling realized gains. Use `calculate_recycling_capacity` to determine additional deployment capacity, `analyze_dpi_impact` to evaluate how recycling affects investor distributions and DPI timing, and `optimize_recycling_rate` to find the ideal reinvestment percentage that maximizes returns while meeting LP liquidity requirements.


## Available Tools (3)
- **analyze_dpi_impact**: Evaluates how recycling gains affects the fund's distribution profile to investors
- **calculate_recycling_capacity**: Determines the total additional capital available for new investments based on recycling decisions
- **optimize_recycling_rate**: Identifies the best recycling percentage to maximize returns while adhering to investor liquidity needs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Fund Recycling Impact** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my additional deployment capacity if I have $50M in realized gains and want to recycle 20%?"

**🤖 AI Agent:**
> Your effective fund size increase is $10,000,000.

---

**👤 You:**
> "How will recycling 30% of $40M gains affect my DPI if I have $200M initial capital and a 5-year reinvestment period?"

**🤖 AI Agent:**
> The projected DPI will be lower than immediate distribution due to the 5-year reinvestment period, delaying the realization of the recycled $12M.

---

**👤 You:**
> "Find the optimal recycling rate for $100M gains, $500M initial capital, $20M fees, and a minimum DPI of 1.2."

**🤖 AI Agent:**
> The optimal recycling rate is 25%, which maintains a projected DPI of 1.25.


## ❓ FAQ

**Q: How does recycling affect my fund's DPI?**
Recycling gains typically delays DPI because capital is held for reinvestment rather than being distributed immediately to LPs. You can use `analyze_dpi_impact` to model this delay.

**Q: Can I find the best recycling rate for my LPs?**
Yes, the `optimize_recycling_rate` tool identifies the highest possible recycling percentage that satisfies your LPs' minimum DPI requirements.

**Q: What is the purpose of the capacity tool?**
The `calculate_recycling_capacity` tool calculates the effective increase in fund size and the remaining deployable capital available for new investments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-fund-recycling-impact](https://vinkius.com/ai-agent-connect/accelerator-fund-recycling-impact)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Fund Recycling Impact** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-fund-recycling-impact` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Fund Recycling Impact** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-fund-recycling-impact": {
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
