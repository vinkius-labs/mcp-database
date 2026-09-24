# Ad Cost Per Click Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ad-cost-per-click-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Calculate advertising efficiency by determining the cost per individual user click.

## Description
This MCP server provides specialized tools for advertising performance analysis. It allows AI agents to calculate the average cost per click using `calculate_cpc`, compare current spending against budget targets with `get_campaign_efficiency_summary`, and aggregate data across multiple time segments using `aggregate_spend_by_period`. Additionally, it can assess if campaign data is statistically significant via `validate_campaign_viability`.


## Available Tools (4)
- **aggregate_spend_by_period**: Aggregates spend and clicks across multiple time segments
- **calculate_cpc**: Calculates the average cost per click
- **get_campaign_efficiency_summary**: Compares actual CPC to a target efficiency
- **validate_campaign_viability**: Checks if a campaign meets the minimum activity threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ad Cost Per Click Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the average cost for each click if we spent $500 and got 250 clicks?"

**🤖 AI Agent:**
> The average cost per click was $2.00.

---

**👤 You:**
> "Is our campaign efficient if we spent $100 for 50 clicks and our target CPC is $1.50?"

**🤖 AI Agent:**
> No, the actual CPC is $2.00, which is $0.50 above your target budget.

---

**👤 You:**
> "Check if a campaign with 15 clicks is viable if the minimum threshold is 20 clicks."

**🤖 AI Agent:**
> The campaign is not currently viable as it has not met the minimum threshold of 20 clicks.


## ❓ FAQ

**Q: How is the cost per click calculated?**
The cost per click is determined by dividing the total ad spend by the total number of clicks received.

**Q: Can I compare my actual spend to a target budget?**
Yes, you can use `get_campaign_efficiency_summary` to compare your actual CPC against a target value to see if you are within budget.

**Q: How do I know if my campaign data is reliable?**
You can use `validate_campaign_viability` to check if the current click volume meets your minimum threshold for statistical significance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ad-cost-per-click-analytics](https://vinkius.com/en/ai-agent-connect/ad-cost-per-click-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ad Cost Per Click Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ad-cost-per-click-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ad Cost Per Click Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ad-cost-per-click-analytics": {
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
