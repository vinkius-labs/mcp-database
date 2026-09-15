# Product Usage & Engagement Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/product-usage-engagement-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [product-management](../categories/product-management.md)

Analyze product stickiness, engagement scores, and user retention correlations.

## Description
This MCP server provides a specialized suite of analytical tools to measure product health and user behavior. It connects your AI agents to deep engagement metrics, allowing for automated analysis of stickiness, user interaction depth, and retention patterns. Use `get_stickiness_metrics` to calculate the DAU/MAU ratio, `calculate_engagement_score` to synthesize user activity into a single health metric, `analyze_retention_correlation` to see if engagement drives longevity, and `generate_power_user_distribution` to identify your most active user segments.


## Available Tools (4)
- **analyze_retention_correlation**: Determines if higher engagement is effectively driving user retention
- **calculate_engagement_score**: Generates a single score representing the depth of user interaction
- **generate_power_user_distribution**: Provides a breakdown of user activity levels to identify the power user density
- **get_stickiness_metrics**: Calculates the product's daily stickiness ratio


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Product Usage & Engagement Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the stickiness ratio for a product with 500 DAU and 5000 MAU?"

**🤖 AI Agent:**
> The stickiness ratio is 0.1, which represents a 10% stickiness level.

---

**👤 You:**
> "Calculate the engagement score for a session lasting 15 minutes with 20 actions and a 0.5 feature adoption rate."

**🤖 AI Agent:**
> The synthesized engagement score is 75, which falls into the High Engagement category.

---

**👤 You:**
> "Analyze the correlation between these engagement scores [0.8, 0.6, 0.4] and retention rates [0.5, 0.3, 0.1]."

**🤖 AI Agent:**
> The correlation coefficient is 1.0, indicating a Strong and statistically significant relationship between engagement and retention.


## ❓ FAQ

**Q: How do I calculate my product's stickiness?**
You can use the `get_stickiness_metrics` tool by providing your Daily Active Users (DAU) and Monthly Active Users (MAU).

**Q: Can I identify my power users?**
Yes, the `generate_power_user_distribution` tool provides a breakdown of activity levels and identifies the ratio of power users within a 30-day window.

**Q: How is the engagement score determined?**
The `calculate_engagement_score` tool synthesizes session duration, action density, and feature adoption rates into a single score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/product-usage-engagement-engine](https://vinkius.com/en/ai-agent-connect/product-usage-engagement-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Product Usage & Engagement Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `product-usage-engagement-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Product Usage & Engagement Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "product-usage-engagement-engine": {
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
