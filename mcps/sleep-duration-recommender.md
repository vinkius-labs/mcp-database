# Sleep Duration Recommender MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sleep-duration-recommender)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Get personalized sleep recommendations based on age, activity, and health.

## Description
This MCP server provides precise sleep guidance by analyzing individual biological and lifestyle factors. It uses NSF guidelines to establish a baseline and then adjusts targets based on physical activity and health conditions. You can use `get_age_based_range` to find standard age-based sleep windows, `calculate_personalized_target` for a specific daily goal, `calculate_deficit_adjustment` to plan recovery from sleep debt, or `generate_weekly_sleep_budget` for a complete seven-day plan.


## Available Tools (4)
- **get_age_based_range**: Retrieves the baseline sleep duration range recommended by the NSF for a specific age
- **calculate_deficit_adjustment**: Calculates how much extra sleep is needed to compensate for existing sleep debt
- **calculate_personalized_target**: Determines a specific, single sleep hour target by adjusting the age-based range with lifestyle factors
- **generate_weekly_sleep_budget**: Provides a comprehensive weekly sleep plan that combines baseline needs and debt recovery


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Duration Recommender** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am 30 years old with a high activity level. How much sleep do I need?"

**🤖 AI Agent:**
> Based on your age and high activity level, your personalized sleep target is 8.5 hours per night.

---

**👤 You:**
> "I have a 5-hour sleep debt. How should I adjust my sleep to recover?"

**🤖 AI Agent:**
> To recover your 5-hour debt, you should add 45 minutes of sleep to your daily target for the next 7 days.

---

**👤 You:**
> "Give me a weekly sleep plan for a 45-year-old with moderate activity and 2 hours of sleep debt."

**🤖 AI Agent:**
> Your total weekly sleep budget is 57.5 hours, with a recommended daily target of 8 hours and 15 minutes.


## ❓ FAQ

**Q: How does activity level affect my sleep recommendation?**
Higher physical activity increases your body's need for recovery, which shifts your `calculate_personalized_target` result toward a higher number of sleep hours.

**Q: Can I recover from sleep debt quickly?**
The `calculate_deficit_adjustment` tool calculates a safe daily increase to your sleep target, distributing the recovery over several days to ensure it is manageable.

**Q: What are the baseline sleep guidelines used?**
The server uses the National Sleep Foundation (NSF) guidelines to determine the initial age-based sleep range.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sleep-duration-recommender](https://vinkius.com/en/ai-agent-connect/sleep-duration-recommender)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Duration Recommender** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-duration-recommender` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Duration Recommender** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-duration-recommender": {
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
