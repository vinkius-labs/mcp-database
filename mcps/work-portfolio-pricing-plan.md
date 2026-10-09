# Work Portfolio Pricing Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/work-portfolio-pricing-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A precision pricing engine for calculating service quotes based on labor, complexity, and margins.

## Description
This MCP server provides a suite of tools to automate professional service pricing. It calculates base labor costs using `get_labor_cost`, generates comprehensive quotes with `calculate_total_quote`, verifies client budget alignment with `validate_budget_fit`, and produces itemized client reports via `summarize_pricing_breakdown`. It is designed to bridge the gap between project complexity and accurate financial forecasting.


## Available Tools (4)
- **summarize_pricing_breakdown**: Provides a detailed itemized view of the pricing components for client presentation
- **validate_budget_fit**: Checks if a calculated quote aligns with a client's predefined budget tier
- **calculate_total_quote**: Generates a comprehensive final price including labor, revisions, third-party costs, and profit margins
- **get_labor_cost**: Determines the base cost of professional labor required for a specific set of deliverables


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Work Portfolio Pricing Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the labor cost for deliverables with weights 5, 10, and 3 at an hourly rate of 150."

**🤖 AI Agent:**
> The total estimated hours is 18, and the base labor cost is 2700.

---

**👤 You:**
> "Generate a quote with a base labor cost of 5000, third-party costs of 500, a 30% target margin, 2 included revisions, 4 requested revisions, and a 100 surcharge per extra revision."

**🤖 AI Agent:**
> The final price is 7150, with a profit amount of 1650.

---

**👤 You:**
> "Is a quote of 4500 within the 'mid' budget tier?"

**🤖 AI Agent:**
> The price is within the budget for the mid tier.


## ❓ FAQ

**Q: How does the tool calculate labor costs?**
The `get_labor_cost` tool calculates the total cost by multiplying the sum of deliverable complexity weights by the provided hourly rate.

**Q: Can I check if a quote fits a specific client budget?**
Yes, use the `validate_budget_fit` tool to compare the final price against predefined budget tiers like low, mid, or high.

**Q: How are extra revisions handled?**
When using `calculate_total_quote`, you can specify the number of included revisions and a surcharge for any additional requested revisions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/work-portfolio-pricing-plan](https://vinkius.com/en/ai-agent-connect/work-portfolio-pricing-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Work Portfolio Pricing Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `work-portfolio-pricing-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Work Portfolio Pricing Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "work-portfolio-pricing-plan": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
