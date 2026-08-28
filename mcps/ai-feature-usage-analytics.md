# AI Feature Usage Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ai-feature-usage-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Analyze AI feature stickiness, usage distribution, and engagement trajectories.

## Description
This MCP server provides deep insights into how users interact with AI capabilities. It allows AI agents to calculate stickiness via `get_stickiness_metrics`, analyze usage intensity with `get_usage_distribution`, track engagement trends using `get_engagement_trajectory`, and compare behavior across tiers with `get_segment_comparison`.


## Available Tools (4)
- **get_engagement_trajectory**: Determines the direction and velocity of AI engagement
- **get_segment_comparison**: Compares AI engagement metrics across different user tiers
- **get_stickiness_metrics**: Calculates the stickiness ratio (DAU/MAU) for a specific user segment
- **get_usage_distribution**: Analyzes the distribution of AI usage intensities across users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AI Feature Usage Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the stickiness ratio for the pro segment with 500 daily users and 2000 monthly users?"

**🤖 AI Agent:**
> The stickiness ratio for the pro segment is 0.25.

---

**👤 You:**
> "Is engagement improving for the enterprise segment if sessions went from 100 to 150?"

**🤖 AI Agent:**
> Yes, the engagement trajectory is improving with a growth rate of 50.0%.

---

**👤 You:**
> "Show me the usage distribution for text-generation with sessions [1, 5, 10, 20, 50]."

**🤖 AI Agent:**
> The distribution for text-generation is: low-frequency: 3 users, medium-frequency: 1 user, high-frequency: 1 user.


## ❓ FAQ

**Q: How is stickiness calculated?**
Stickiness is calculated using the `get_stickiness_metrics` tool, which divides daily active users by monthly active users.

**Q: Can I compare different user tiers?**
Yes, use `get_segment_comparison` to compare average sessions and stickiness between segments like free, pro, or enterprise.

**Q: What kind of usage distribution data is available?**
The `get_usage_distribution` tool categorizes users into low, medium, and high-frequency buckets based on their session counts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ai-feature-usage-analytics](https://vinkius.com/ai-agent-connect/ai-feature-usage-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AI Feature Usage Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ai-feature-usage-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AI Feature Usage Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ai-feature-usage-analytics": {
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
