# Runway Calculation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/runway-calculation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate startup runway, zero cash dates, and financial warning thresholds.

## Description
This MCP server provides essential financial modeling tools for startups to monitor their operational lifespan. Use `get_runway_projection` to determine how many months of cash remain, or `get_runway_warning_status` to identify if the company is entering a critical financial phase. You can also use `simulate_cost_reduction` to model how cutting expenses extends your runway, or `get_revenue_growth_impact` to see how different growth scenarios change your financial outlook.


## Available Tools (4)
- **get_runway_warning_status**: Identifies if the company is approaching critical financial milestones
- **get_revenue_growth_impact**: Determines the impact of varying growth rates on the total runway
- **get_runway_projection**: Calculates core runway metrics based on current financials and growth
- **simulate_cost_reduction**: Models how much the runway would extend if operating expenses are reduced


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Runway Calculation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much runway do I have with $500,000 cash, $50,000 monthly burn, $10,000 monthly revenue, and 5% monthly growth?"

**🤖 AI Agent:**
> Based on your current financials, you have approximately 12.4 months of runway remaining.

---

**👤 You:**
> "What is my runway status if I have $200,000 cash, $40,000 burn, and $5,000 revenue with 2% growth?"

**🤖 AI Agent:**
> Your current status is Critical because your runway is less than 6 months.

---

**👤 You:**
> "How much would my runway extend if I reduce my $50,000 monthly burn by $10,000?"

**🤖 AI Agent:**
> Reducing your monthly burn by $10,000 would extend your runway by 4.5 months.


## ❓ FAQ

**Q: How do I calculate my runway?**
You can use the `get_runway_projection` tool by providing your current cash balance, monthly burn, monthly revenue, and expected revenue growth rate.

**Q: What does a 'Critical' status mean?**
A 'Critical' status is triggered when the `get_runway_warning_status` tool determines that the remaining runway is less than 6 months.

**Q: Can I simulate cost-cutting measures?**
Yes, use the `simulate_cost_reduction` tool to see how much your runway extends if you reduce your monthly burn by a specific amount.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/runway-calculation](https://vinkius.com/en/ai-agent-connect/runway-calculation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Runway Calculation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `runway-calculation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Runway Calculation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "runway-calculation": {
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
