# Bottling Line Changeover Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bottling-line-changeover-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Quantify changeover duration and cost using SMED principles.

## Description
This MCP server provides specialized tools for beverage production managers to calculate the economic impact of product transitions. By applying SMED (Single Minute Exchange of Dies) methodology, it helps identify downtime costs and optimization opportunities. Use `get_changeover_metrics` to calculate total duration and cost, `analyze_smed_opportunities` to find ways to convert internal tasks to external ones, `evaluate_product_transition` to assess complexity based on bottle size and closure types, and `calculate_labor_efficiency` to model the impact of crew size on production speed.


## Available Tools (4)
- **get_changeover_metrics**: Calculates the total estimated duration and economic cost of a specific changeover
- **calculate_labor_efficiency**: Determines the impact of crew size on the changeover duration
- **analyze_smed_opportunities**: Identifies specific tasks that can be converted from internal to external to reduce downtime
- **evaluate_product_transition**: Estimates the complexity level and estimated base duration of a transition based on physical attributes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bottling Line Changeover Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the cost for a changeover from Product A to Product B with a line speed of 5000 units/hour and 3 tasks."

**🤖 AI Agent:**
> The total changeover duration is 45 minutes, resulting in a downtime cost of $3,750.00.

---

**👤 You:**
> "How much time can I save if I move the 'Tooling Swap' task to be an external task?"

**🤖 AI Agent:**
> By converting the 'Tooling Swap' to an external task, you can achieve a potential time savings of 25 minutes.

---

**👤 You:**
> "What is the complexity of switching from a 500ml screw cap bottle to a 1L crown cork bottle?"

**🤖 AI Agent:**
> The transition has a high complexity score due to changes in both bottle size and closure type.


## ❓ FAQ

**Q: How does this tool help reduce downtime?**
It uses `analyze_smed_opportunities` to identify internal tasks that can be moved to external preparation, reducing the time the line is actually stopped.

**Q: Can I account for different crew sizes?**
Yes, you can use `calculate_labor_efficiency` to determine how adding more personnel affects the optimized changeover duration.

**Q: What factors influence the complexity score?**
The `evaluate_product_transition` tool calculates complexity based on changes in bottle size, closure type, and labeling systems.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bottling-line-changeover-optimizer](https://vinkius.com/en/ai-agent-connect/bottling-line-changeover-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bottling Line Changeover Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bottling-line-changeover-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bottling Line Changeover Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bottling-line-changeover-optimizer": {
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
