# Mining Project NPV Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mining-project-npv-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Financial feasibility analysis for mining projects using DCF modeling.

## Description
This MCP server provides a complete suite of financial tools for evaluating mining operations. It uses discounted cash flow (DCF) modeling to calculate critical indicators like NPV, IRR, and payback period. Users can use `calculate_project_metrics` to get a full financial profile, `compare_scenarios` to evaluate different project configurations, `analyze_sensitivity` to test how variables like metal price affect value, and `calculate_break_even_price` to find the minimum profitable price point.


## Available Tools (4)
- **analyze_sensitivity**: Determines how sensitive the NPV is to changes in a single specific variable
- **calculate_break_even_price**: Identifies the minimum metal price required to achieve a zero NPV
- **calculate_project_metrics**: Provides a full suite of primary financial indicators for a single mining project scenario
- **compare_scenarios**: Evaluates the relative performance of two different project configurations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mining Project NPV Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the NPV and IRR for a project with 100M CAPEX, 50 OPEX per unit, a production of 10,000 units for 5 years, a metal price of 150, a 10% discount rate, 30% tax, 5% royalty, and 10M annual depreciation."

**🤖 AI Agent:**
> The project has an NPV of $125,450,000 and an IRR of 18.5%. The payback period is 3.2 years.

---

**👤 You:**
> "What is the break-even metal price for a project with 50M CAPEX and 40 OPEX per unit?"

**🤖 AI Agent:**
> The minimum metal price required to achieve a zero NPV is $85.50 per unit.

---

**👤 You:**
> "How sensitive is the NPV to a 10% increase in metal price?"

**🤖 AI Agent:**
> A 10% increase in metal price results in an NPV of $145,000,000, compared to the base NPV of $125,450,000.


## ❓ FAQ

**Q: What metrics does this server calculate?**
The server calculates Net Present Value (NPV), Internal Rate of Return (IRR), payback period, and total project value using `calculate_project_metrics`.

**Q: How can I compare two different mining scenarios?**
You can use the `compare_scenarios` tool by providing the parameter sets for both scenarios as JSON strings.

**Q: Can I find the minimum price needed to make a project viable?**
Yes, the `calculate_break_even_price` tool identifies the minimum metal price required to achieve a zero NPV.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mining-project-npv-analysis](https://vinkius.com/en/ai-agent-connect/mining-project-npv-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mining Project NPV Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mining-project-npv-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mining Project NPV Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mining-project-npv-analysis": {
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
