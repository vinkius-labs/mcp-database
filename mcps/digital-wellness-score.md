# Digital Wellness Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/digital-wellness-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze screen time data to assess digital health and addiction risk.

## Description
This MCP server transforms raw screen activity into actionable wellness metrics. It analyzes usage patterns to calculate an overall health score, identify addiction risks, and provide personalized recommendations. Use `get_overall_wellness` for a high-level summary, `get_category_breakdown` to see time distribution, `assess_addiction_risk` to evaluate compulsive usage, and `get_personalized_recommendations` for specific tips to improve your digital habits.


## Available Tools (4)
- **assess_addiction_risk**: Specifically evaluates the likelihood of compulsive device usage
- **get_category_breakdown**: Detailed analysis of how time is distributed across different digital activities
- **get_overall_wellness**: Provides a high-level summary of the user's current digital health status
- **get_personalized_recommendations**: Generates actionable advice to improve digital wellness based on user behavior


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Digital Wellness Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current digital health status based on 300 minutes of screen time, 50 pickups, and 20 minutes of bedtime use?"

**🤖 AI Agent:**
> Your current health status is Healthy, with an overall wellness score of 75/100.

---

**👤 You:**
> "Show me the breakdown of my screen time usage."

**🤖 AI Agent:**
> You spent 60% of your time in Productive categories and 40% in Leisure categories.

---

**👤 You:**
> "Am I at risk of digital addiction?"

**🤖 AI Agent:**
> Your addiction risk level is Low, as your pickups are well-distributed throughout the day.


## ❓ FAQ

**Q: How is the wellness score calculated?**
The score balances productive time against interruptions like high pickup frequency, notification volume, and usage during sleep hours.

**Q: Can I get specific tips to reduce my screen time?**
Yes, you can use `get_personalized_recommendations` to receive actionable tips and suggested usage limits based on your behavior.

**Q: What determines the addiction risk level?**
Risk is primarily driven by the density of device pickups and the amount of time spent in leisure-based categories.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/digital-wellness-score](https://vinkius.com/en/ai-agent-connect/digital-wellness-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Digital Wellness Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `digital-wellness-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Digital Wellness Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "digital-wellness-score": {
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
