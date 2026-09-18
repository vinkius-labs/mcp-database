# Daily Water Intake Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/daily-water-intake-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Personalized daily hydration recommendations based on weight, activity, and climate.

## Description
This MCP server provides precise hydration guidance by calculating water requirements through several physiological and environmental lenses. Using `calculate_daily_intake`, users receive a total volume recommendation that accounts for their body weight, physical activity levels, and local climate. The server also offers `get_hydration_schedule` to distribute water intake throughout the day, ensuring optimal hydration without sleep disruption. It specifically handles adjustments for pregnancy and breastfeeding to support unique biological needs.


## Available Tools (4)
- **get_climate_adjustment**: Retrieve the specific adjustment needed for environmental conditions
- **calculate_daily_intake**: Calculate the total recommended daily water intake based on various factors
- **get_activity_factor**: Retrieve the specific multiplier or additive volume used to adjust for physical activity
- **get_hydration_schedule**: Provide a structured timing recommendation for consuming water throughout the day


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Daily Water Intake Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much water should I drink daily? I weigh 70kg, I am moderately active, and live in a hot climate."

**🤖 AI Agent:**
> Based on your weight of 70kg, moderate activity, and hot climate, your recommended daily water intake is 3200ml.

---

**👤 You:**
> "Create a drinking schedule for 2500ml of water. I wake up at 07:00 and sleep at 23:00."

**🤖 AI Agent:**
> Here is your hydration schedule: 07:00 - 300ml, 09:00 - 400ml, 11:00 - 400ml, 13:00 - 400ml, 15:00 - 400ml, 17:00 - 300ml, 19:00 - 300ml.

---

**👤 You:**
> "I am 60kg and breastfeeding. What is my daily water requirement in a temperate climate?"

**🤖 AI Agent:**
> Your recommended daily water intake is 2850ml, accounting for your weight, breastfeeding status, and temperate climate.


## ❓ FAQ

**Q: How does the calculator account for physical activity?**
The `calculate_daily_intake` tool applies specific multipliers based on whether your activity level is sedentary, moderate, or active to compensate for fluid loss.

**Q: Can I get a schedule for when to drink water?**
Yes, you can use the `get_hydration_schedule` tool to generate a structured plan for consuming your target water volume between your wake-up and sleep times.

**Q: Does it support pregnancy and breastfeeding adjustments?**
Yes, the `calculate_daily_intake` tool includes specific logic to increase water recommendations for users who are pregnant or breastfeeding.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/daily-water-intake-calculator](https://vinkius.com/en/ai-agent-connect/daily-water-intake-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Daily Water Intake Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `daily-water-intake-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Daily Water Intake Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "daily-water-intake-calculator": {
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
