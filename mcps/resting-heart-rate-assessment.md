# Resting Heart Rate Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/resting-heart-rate-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Analyze cardiovascular health and fitness trends using resting heart rate data.

## Description
This MCP server provides deep insights into cardiovascular health by analyzing resting heart rate (RHR). It calculates percentile rankings, fitness indicators, and training recommendations while accounting for age, gender, and medical factors like beta-blocker use. Use `get_rhr_status` for a primary health assessment, `get_fitness_trend` to track improvements, `get_training_recommendations` for actionable advice, and `get_comparative_percentile` to see how you rank against specific demographics.


## Available Tools (4)
- **get_comparative_percentile**: Calculates how the user's RHR compares to a specific demographic subset
- **get_fitness_trend**: Analyzes how the current RHR compares to a provided historical RHR to determine trends
- **get_rhr_status**: Provides a primary health assessment of the user's current RHR
- **get_training_recommendations**: Provides actionable training advice based on the current cardiovascular status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Resting Heart Rate Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My resting heart rate is 55, I am 30 years old, male, and an athlete. I am not on any medication. What is my status?"

**🤖 AI Agent:**
> Your cardiovascular fitness is Excellent, placing you in the top percentile for your age and gender.

---

**👤 You:**
> "I am 45, female, sedentary, and I take beta-blockers. My RHR is 62. How should I train?"

**🤖 AI Agent:**
> Given your medication, focus on gradual zone 2 training to build a steady aerobic base safely.

---

**👤 You:**
> "My RHR was 65 last month and it is 60 today. What does this mean?"

**🤖 AI Agent:**
> Your cardiovascular efficiency is improving.


## ❓ FAQ

**Q: How does beta-blocker use affect the assessment?**
Beta-blockers can artificially lower your heart rate. The `get_rhr_status` tool detects this and adjusts the fitness indicator to ensure your cardiovascular capacity isn't misinterpreted.

**Q: Can I track my fitness progress over time?**
Yes, you can use the `get_fitness_trend` tool to compare your current resting heart rate with previous measurements to see if your efficiency is improving.

**Q: What kind of training advice is provided?**
The `get_training_recommendations` tool provides specific guidance, such as focusing on zone 2 training for sedentary users or maintaining aerobic base for athletes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/resting-heart-rate-assessment](https://vinkius.com/en/ai-agent-connect/resting-heart-rate-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Resting Heart Rate Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `resting-heart-rate-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Resting Heart Rate Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "resting-heart-rate-assessment": {
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
