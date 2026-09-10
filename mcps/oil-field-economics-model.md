# Oil Field Economics Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/oil-field-economics-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Perform detailed economic analysis for oil field developments using DCF modeling.

## Description
This MCP server provides a complete suite of tools for oil and gas economic evaluation. It uses discounted cash flow (DCF) modeling to calculate critical financial metrics including NPV, IRR, payout period, and ROI. Users can model complex production profiles, account for inflation, and apply specific fiscal terms like royalties and taxes. The server includes tools to `calculate_project_economics` for single scenarios, `run_sensitivity_analysis` to test variable volatility, `get_production_summary` for physical output analysis, and `compare_scenarios` to evaluate competing development strategies.


## Available Tools (4)
- **compare_scenarios**: Compares two different development scenarios
- **get_production_summary**: Provides a high-level overview of the physical production characteristics
- **run_sensitivity_analysis**: Evaluates how changes in key variables impact the project NPV
- **calculate_project_economics**: Calculates core economic metrics (NPV, IRR, Payout, ROI) for a single development scenario


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Oil Field Economics Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the economics for a project with 500M CAPEX, 50M annual OPEX, and a 10% discount rate."

**🤖 AI Agent:**
> The project has an NPV of $125,400,000, an IRR of 14.2%, a payout period of 6.5 years, and an ROI of 1.25.

---

**👤 You:**
> "What is the peak production for a profile with volumes of 100, 200, 150, and 50 units per year?"

**🤖 AI Agent:**
> The peak production is 200 units, occurring in year 2.

---

**👤 You:**
> "Run a sensitivity analysis on CAPEX with a variance of -10% and +10%."

**🤖 AI Agent:**
> At -10% CAPEX, the NPV is $150,000,000. At +10% CAPEX, the NPV is $100,000,000.


## ❓ FAQ

**Q: What metrics can I calculate?**
You can calculate Net Present Value (NPV), Internal Rate of Return (IRR), the project payout period, and Return on Investment (ROI) using `calculate_project_economics`.

**Q: How do I test how oil price changes affect my project?**
Use the `run_sensitivity_analysis` tool. You provide your base scenario and specify 'oilPrice' as the variable to vary along with a range of percentage deviations.

**Q: Can I compare two different development plans?**
Yes, the `compare_scenarios` tool allows you to input two different development scenarios to determine which is more economically viable based on NPV.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/oil-field-economics-model](https://vinkius.com/ai-agent-connect/oil-field-economics-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Oil Field Economics Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `oil-field-economics-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Oil Field Economics Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oil-field-economics-model": {
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
