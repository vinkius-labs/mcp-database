# Gacha Spark Point Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/gacha-spark-point-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Predict if you will reach your gacha spark guarantee based on current progress and daily pull velocity.

## Description
This MCP server provides deterministic tools to track gacha progress toward a 'Spark' guarantee. Use `calculate_spark_projection` to forecast your total points at the end of a banner, determine if you will successfully hit your threshold, and calculate exactly how many pulls and days are required to reach it. It also includes `get_spark_status_summary` for quick progress checks and `validate_pull_capacity` to verify if your current daily pulling rate is sufficient to meet your goals before the banner expires.


## Available Tools (3)
- **calculate_spark_projection**: Predicts whether a user will reach their target and determines the remaining effort required
- **get_spark_status_summary**: Provides a high-level verification of a user's progress against the threshold
- **validate_pull_capacity**: Checks if a user's planned daily pulling rate is sufficient to hit a goal within a specific timeframe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gacha Spark Point Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 150 spark points, I do 10 pulls per day, and there are 20 days left. My target is 300. Will I make it?"

**🤖 AI Agent:**
> Yes, you will reach your goal. You are projected to have 350 points at the end of the banner, which exceeds your 300 point threshold.

---

**👤 You:**
> "How many more pulls do I need to reach a 200 spark threshold if I currently have 50 points?"

**🤖 AI Agent:**
> You need 150 more pulls to reach the 200 spark threshold.

---

**👤 You:**
> "I need 100 more pulls and I have 5 days left. I can do 15 pulls per day. Can I reach my goal?"

**🤖 AI Agent:**
> Yes, you can reach your goal. At 15 pulls per day, you will complete the required pulls in 7 days, but since you only need 100 pulls, you will actually finish in 7 days? Wait, 100/15 is 6.66, so 7 days. If you only have 5 days, you will fall short by 25 pulls.


## ❓ FAQ

**Q: How do I know if I will reach my spark goal?**
You can use the `calculate_spark_projection` tool. By providing your current points, daily pulls, and days remaining, it will tell you if your projected points meet the threshold.

**Q: Can I check my current progress percentage?**
Yes, the `get_spark_status_summary` tool provides your current progress percentage and the exact number of points remaining to hit the threshold.

**Q: What if my daily pulls change?**
You should update your `pullsPerDay` input in the tools to reflect your new rate. This ensures the projection and capacity validation remain accurate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/gacha-spark-point-tracker](https://vinkius.com/ai-agent-connect/gacha-spark-point-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gacha Spark Point Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gacha-spark-point-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gacha Spark Point Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gacha-spark-point-tracker": {
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
