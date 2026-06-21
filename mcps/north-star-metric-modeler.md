# North Star Metric Modeler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/north-star-metric-modeler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Decompose North Star Metrics into actionable driver trees and simulate growth scenarios.

## Description
The North Star Metric Modeler is a strategic planning tool designed to bridge the gap between high-level objectives and actionable growth levers. By using tools like `set_north_star_goal`, you can establish your current performance and target milestones. The engine allows you to define structural relationships via `configure_driver_tree`, assigning weights to key pillars such as Acquisition, Activation, Engagement, Retention, and Monetization. Once configured, you can use `simulate_lever_improvement` to predict how specific changes in these pillars will impact your overall metric, or use `calculate_contribution_distribution` to identify which levers are most critical for closing the gap between your current state and your target.


## Available Tools (4)
- **set_north_star_goal**: Establishes the primary objective
- **simulate_lever_improvement**: Predicts impact of pillar improvement
- **calculate_contribution_distribution**: Analyzes contribution of each pillar to the gap
- **configure_driver_tree**: Total weight must be 100%.

Defines the structural relationship between NSM and pillars


## 💬 Prompt Examples

Here are some examples of how you can interact with the **North Star Metric Modeler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 10,000 Monthly Active Users and my goal is 25,000. How much growth do I need?"

**🤖 AI Agent:**
> To reach your target of 25,000 from 10,000, you require a total growth of 15,000 users, which represents a 150% increase.

---

**👤 You:**
> "If I improve my Retention pillar by 20%, what will be the new North Star Metric value?"

**🤖 AI Agent:**
> A 20% improvement in your Retention pillar will result in a projected North Star Metric of 12,500 users.

---

**👤 You:**
> "Which pillars are contributing most to my growth gap?"

**🤖 AI Agent:**
> Based on your current configuration, the Acquisition pillar is responsible for 40% of the required growth, followed by Engagement at 30%.


## ❓ FAQ

**Q: How do I start modeling my metric?**
Start by using the `set_north_star_goal` tool to define your current value, target value, and the name of your North Star Metric.

**Q: How do I assign importance to different growth pillars?**
Use the `configure_driver_tree` tool. You must provide a JSON array of pillar assignments and an array of corresponding weights that sum up to exactly 100%.

**Q: Can I predict the impact of a specific growth initiative?**
Yes, use `simulate_lever_improvement` by specifying the pillar name and the projected percentage increase to see its effect on your North Star Metric.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/north-star-metric-modeler](https://vinkius.com/mcp/north-star-metric-modeler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **North Star Metric Modeler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `north-star-metric-modeler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **North Star Metric Modeler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "north-star-metric-modeler": {
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
