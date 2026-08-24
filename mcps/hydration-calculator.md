# Hydration Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hydration-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Personalized daily water intake recommendations based on weight, activity, and environment.

## Description
This MCP server provides precise hydration planning by calculating daily water requirements. It accounts for baseline physiological needs based on body mass, adjustments for physical activity, environmental factors like heat or humidity, and special physiological states such as pregnancy or breastfeeding. Use `calculate_daily_hydration` to get a full breakdown of your needs in milliliters, ounces, and cups, or use `get_hydration_thresholds` to understand your baseline range.


## Available Tools (3)
- **calculate_daily_hydration**: Provides a comprehensive daily water intake recommendation based on a user's specific profile
- **compare_activity_impact**: Answers how much extra water is required to move between different levels of physical exertion
- **get_hydration_thresholds**: Answers what the minimum and maximum weight-based baseline requirements are for a given weight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hydration Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I weigh 70kg, I am a moderate activity level, and I live in a hot climate. How much water should I drink?"

**🤖 AI Agent:**
> Based on your profile, you should drink 2600ml of water per day. This includes a baseline of 2100ml, a 500ml adjustment for the hot climate, and your activity level.

---

**👤 You:**
> "What is the difference in water needs if I increase my exercise from 30 to 60 minutes?"

**🤖 AI Agent:**
> Increasing your exercise duration from 30 to 60 minutes will require an additional 500ml of water.

---

**👤 You:**
> "I am 150lbs and breastfeeding. How much water do I need daily?"

**🤖 AI Agent:**
> Your daily water requirement is approximately 2450ml, which is about 83 ounces or 10 cups.


## ❓ FAQ

**Q: How does activity level affect my water needs?**
Physical exertion increases fluid loss. The `calculate_daily_hydration` tool adds 500ml for every 30 minutes of exercise to compensate for sweat loss.

**Q: Can I calculate my baseline hydration without exercise data?**
Yes, you can use `get_hydration_thresholds` to find the minimum and maximum baseline requirements based solely on your body weight.

**Q: Does the calculator account for pregnancy?**
Yes, the `calculate_daily_hydration` tool includes a 300ml increase if you indicate you are pregnant to support increased blood volume and fetal development.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hydration-calculator](https://vinkius.com/ai-agent-connect/hydration-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hydration Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hydration-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hydration Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hydration-calculator": {
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
