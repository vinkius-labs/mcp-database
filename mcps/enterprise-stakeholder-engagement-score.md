# Enterprise Stakeholder Engagement Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-stakeholder-engagement-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [enterprise](../categories/enterprise.md)

Analyze stakeholder relationship health, momentum, and risks.

## Description
This MCP server provides advanced analytical tools to measure the quality and momentum of stakeholder relationships. Use `calculate_engagement_score` to determine the qualitative health of your engagement, `calculate_engagement_velocity` to track relationship trends, `identify_engagement_risks` to flag critical stakeholders needing attention, and `summarize_stakeholder_landscape` for a high-level overview of influence and engagement distribution.


## Available Tools (4)
- **calculate_engagement_score**: Calculates the current qualitative health of stakeholder engagement
- **calculate_engagement_velocity**: Calculates the rate of change in engagement over time
- **identify_engagement_risks**: Identifies stakeholders requiring immediate attention based on thresholds
- **summarize_stakeholder_landscape**: Provides a high-level breakdown of stakeholder influence and engagement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Stakeholder Engagement Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current qualitative health of our stakeholder engagement?"

**🤖 AI Agent:**
> The current engagement score is 78, with a weighted average depth of 0.75 and a weighted average sentiment of 0.4.

---

**👤 You:**
> "Are there any stakeholders that require immediate attention?"

**🤖 AI Agent:**
> Yes, stakeholder ID 'SH-992' is flagged as High Severity due to low sentiment and high importance.

---

**👤 You:**
> "Give me a high-level breakdown of our stakeholder landscape."

**🤖 AI Agent:**
> There are 15 total stakeholders, with 3 high-influence individuals and an average engagement score of 65.


## ❓ FAQ

**Q: How is the engagement score calculated?**
The score is a normalized value from 0 to 100, calculated by weighting stakeholder importance and influence against meeting frequency, engagement depth, and sentiment scores.

**Q: Can I identify high-risk stakeholders?**
Yes, using `identify_engagement_risks`, you can flag stakeholders whose engagement depth or sentiment falls below your custom thresholds, especially those with high importance.

**Q: What does engagement velocity represent?**
Engagement velocity measures the rate of change in engagement quality between two periods, indicating if relationships are strengthening or declining.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-stakeholder-engagement-score](https://vinkius.com/ai-agent-connect/enterprise-stakeholder-engagement-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Stakeholder Engagement Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-stakeholder-engagement-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Stakeholder Engagement Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-stakeholder-engagement-score": {
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
