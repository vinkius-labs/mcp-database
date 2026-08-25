# Accelerator Alumni Engagement MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-alumni-engagement)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business](../categories/business.md)

Measures alumni engagement effectiveness through scoring, trends, and economic value.

## Description
This MCP server provides tools to evaluate the health and economic impact of accelerator alumni networks. It calculates a comprehensive engagement score by analyzing active alumni percentages, mentor participation, event attendance, and referral rates. Use `get_engagement_summary` to obtain a high-level overview of engagement health and economic value. Analyze community stability using `get_retention_analysis` to track engagement trends over time. Additionally, `get_platform_impact_adjustment` allows for adjusting scores based on whether engagement occurs via digital, in-person, or hybrid mediums.


## Available Tools (3)
- **get_engagement_summary**: Provides a high-level overview of current engagement health and economic impact
- **get_platform_impact_adjustment**: Calculates how different engagement mediums influence the overall score
- **get_retention_analysis**: Analyzes the stability and trajectory of the alumni community


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Alumni Engagement** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current engagement health if active alumni is 70%, mentor participation is 20%, event attendance is 50%, and referral rate is 15%?"

**🤖 AI Agent:**
> The current engagement score is 42.5, with an estimated engagement value of $42,500 and a stable engagement status.

---

**👤 You:**
> "Analyze the retention trend for scores: 65, 68, 72, 75."

**🤖 AI Agent:**
> The engagement trend is Increasing, with a stability score of 0.85 and low volatility.

---

**👤 You:**
> "Adjust a raw engagement score of 80 for an in-person event with a touchpoint intensity of 5."

**🤖 AI Agent:**
> The adjusted score for the in-person engagement is 92, with an impact factor of 1.15.


## ❓ FAQ

**Q: What metrics are used to calculate the engagement score?**
The score is a weighted combination of active alumni percentage, mentor participation rate, event attendance, and referral rate.

**Q: How can I track if my alumni community is growing or shrinking?**
You can use the `get_retention_analysis` tool, which analyzes historical engagement scores to determine trend direction and stability.

**Q: Does the medium of engagement affect the final score?**
Yes, you can use `get_platform_impact_adjustment` to adjust the raw score based on whether the engagement is digital, in-person, or hybrid.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-alumni-engagement](https://vinkius.com/ai-agent-connect/accelerator-alumni-engagement)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Alumni Engagement** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-alumni-engagement` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Alumni Engagement** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-alumni-engagement": {
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
