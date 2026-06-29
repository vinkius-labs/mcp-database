# Startup Valuation Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/startup-valuation-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate pre-money startup valuations using Berkus, Scorecard, Risk Factor Sum, and DCF methods.

## Description
This MCP server provides a specialized engine for determining early-stage startup valuations. It implements four distinct methodologies: the Berkus method for milestone-based de-risking, the Scorecard method for regional comparability, the Risk Factor Summation method for qualitative risk assessment, and a simplified Discounted Cash Flow (DCF) model for future cash flow projections. Use `berkus_valuation` to value milestones, `scorecard_valuation` to adjust based on market factors, `risk_summation_valuation` to account for twelve specific risk categories, and `dcf_valuation` to estimate present value from projected flows.


## Available Tools (4)
- **scorecard_valuation**: Calculate valuation using the Scorecard method
- **berkus_valuation**: g., prototype, management team).

Calculate valuation using the Berkus method
- **dcf_valuation**: Calculate valuation using the Simplified DCF method
- **risk_summation_valuation**: Calculate valuation using the Risk Summation method


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Startup Valuation Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a Berkus valuation for a startup that has achieved a prototype and a management team, with a max value of $500k per milestone."

**🤖 AI Agent:**
> $1,000,000

---

**👤 You:**
> "Using the Scorecard method, what is the valuation if the median regional valuation is $2,000,000 and the factor weights are: [{'factorName': 'Management', 'weightPercentage': 1.2}, {'factorName': 'Market', 'weightPercentage': 0.8}]?"

**🤖 AI Agent:**
> $2,000,000

---

**👤 You:**
> "What is the present value of cash flows of $100k, $200k, and $300k over 3 years with a discount rate of 15%?"

**🤖 AI Agent:**
> $438,627.19


## ❓ FAQ

**Q: What is the Berkus method?**
The Berkus method assigns a specific dollar value to key milestones achieved, such as a prototype or a strong management team, up to a maximum cap per milestone.

**Q: How does the Risk Factor Summation tool work?**
It starts with a `baseValuation` and adjusts it by summing positive or negative amounts across twelve standard risk categories like Management Risk and Technology Risk.

**Q: Can I use this for DCF analysis?**
Yes, the `dcf_valuation` tool allows you to input projected cash flows and a discount rate to estimate the present value of your startup's future earnings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/startup-valuation-engine](https://vinkius.com/mcp/startup-valuation-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Startup Valuation Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `startup-valuation-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Startup Valuation Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "startup-valuation-engine": {
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
