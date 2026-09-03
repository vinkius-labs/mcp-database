# Enterprise ABM Campaign Effectiveness MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-abm-campaign-effectiveness)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Measure ABM campaign ROI, engagement metrics, and pipeline conversion efficiency.

## Description
This MCP server provides an analytics engine to measure the financial and engagement success of Account-Based Marketing (ABM) initiatives. It correlates multi-channel engagement with pipeline and revenue outcomes. Use `analyze_campaign_roi` to determine financial returns, `calculate_engagement_metrics` to assess engagement efficiency, `evaluate_pipeline_conversion` to track sales opportunity movement, and `track_account_journey_status` to monitor specific account progress through the lifecycle.


## Available Tools (4)
- **calculate_engagement_metrics**: Calculate engagement metrics including cost per engaged account and engagement rate
- **evaluate_pipeline_conversion**: Evaluate the efficiency of turning engaged accounts into sales opportunities
- **track_account_journey_status**: Track the current lifecycle stage and interaction history of a specific target account
- **analyze_campaign_roi**: Calculate the financial return on investment (ROI) for a specific ABM campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise ABM Campaign Effectiveness** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the ROI for campaign CMP-9928?"

**🤖 AI Agent:**
> The ROI for campaign CMP-9928 was 250%, with a total revenue of $500,000 generated from a total spend of $200,000.

---

**👤 You:**
> "How many accounts have we engaged in the current campaign?"

**🤖 AI Agent:**
> The current campaign has engaged 45 target accounts with an engagement rate of 15%.

---

**👤 You:**
> "What is the status of account ACC-445 in campaign CMP-101?"

**🤖 AI Agent:**
> Account ACC-445 is currently in the 'Pipeline' stage and has had 12 total interactions.


## ❓ FAQ

**Q: How is the ABM ROI calculated?**
The ROI is calculated by comparing the total revenue from closed deals attributed to the campaign against the total campaign spend using the `analyze_campaign_roi` tool.

**Q: Can I track individual account progress?**
Yes, you can use `track_account_journey_status` to see the current lifecycle stage and interaction history for a specific target account.

**Q: What metrics are included in engagement analysis?**
The `calculate_engagement_metrics` tool provides the cost per engaged account, the total number of engaged accounts, and the overall engagement rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-abm-campaign-effectiveness](https://vinkius.com/ai-agent-connect/enterprise-abm-campaign-effectiveness)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise ABM Campaign Effectiveness** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-abm-campaign-effectiveness` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise ABM Campaign Effectiveness** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-abm-campaign-effectiveness": {
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
