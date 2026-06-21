# Growth Accounting Framework MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/growth-accounting-framework)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Analyze user movement, retention patterns, and growth efficiency using the Growth Accounting Framework.

## Description
This MCP server provides a complete toolkit for analyzing product growth through the lens of the Growth Accounting Framework. By decomposing changes in your active user base, you can identify exactly how much growth is driven by new acquisitions, how many users are returning after absence (resurrected), and where you are losing momentum (churned). Use `classify_user_flow` to categorize user movement between periods, `calculate_growth_metrics` to compute critical indicators like the Quick Ratio and Stickiness (DAU/MAU), and `evaluate_growth_health` to receive a qualitative diagnosis of your product's sustainability based on industry benchmarks.


## Available Tools
- **calculate_growth_metrics**: Compute growth stability and engagement metrics
- **evaluate_growth_health**: Diagnose growth health status
- **classify_user_flow**: Categorize users into New, Retained, Resurrected, and Churned


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Growth Accounting Framework** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify these users: current=[1, 2, 3], previous=[2, 3, 4], historical=[4, 5]"

**🤖 AI Agent:**
> New: 1, Retained: 2, Resurreted: 0, Churned: 1

---

**👤 You:**
> "Calculate growth metrics for 50 new users, 10 resurrected users, and 20 churned users."

**🤖 AI Agent:**
> Quick Ratio: 3.0, Net Growth: 40, Stickiness: N/A

---

**👤 You:**
> "What is the growth health if my Quick Ratio is 0.5?"

**🤖 AI Agent:**
> Status: Critical. Your churn rate is outpacing your acquisition and resurrection rate, indicating a declining user base.


## ❓ FAQ

**Q: What is the Quick Ratio?**
The Quick Ratio measures growth momentum by evaluating whether the influx of new and resurrected users is outpacing the loss of churned users. A ratio above 1 indicates a growing user base.

**Q: How do I categorize my users?**
You can use the `classify_user_flow` tool. By providing lists of user IDs for the current, previous, and historical periods, the tool will automatically identify New, Retained, Resurrected, and Churned users.

**Q: What does 'Stickiness' represent in this context?**
Stickiness, calculated as the DAU/MAU ratio, represents how frequently users engage with your product within a month. A higher ratio indicates stronger user retention and engagement.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/growth-accounting-framework](https://vinkius.com/mcp/growth-accounting-framework)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Growth Accounting Framework** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `growth-accounting-framework` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Growth Accounting Framework** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "growth-accounting-framework": {
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
