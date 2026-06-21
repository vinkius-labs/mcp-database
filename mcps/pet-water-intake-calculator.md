# Pet Water Intake Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-water-intake-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate optimal daily water intake for dogs and cats based on weight, food type, and temperature.

## Description
The Pet Water Intake Calculator helps pet owners ensure their animals stay hydrated by calculating precise supplemental water needs. By analyzing species (dog or cat), weight, food moisture content (dry, wet, or raw), and ambient temperature, the server provides actionable hydration targets. Use `calculate_daily_intake` to find specific milliliter requirements, `check_dehydration_indicators` to identify physical warning signs like lethargy or skin elasticity changes, and `get_food_moisture_profile` to understand how different diets impact hydration needs.


## Available Tools
- **calculate_daily_intake**: Calculates the total volume of supplemental water (in ml) a pet needs daily
- **check_dehydration_indicators**: Identifies physical warning signs of dehydration
- **get_food_moisture_profile**: Provides moisture content information for each food type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Water Intake Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much water does my 10kg dog need if I feed him dry food and it is 30 degrees Celsius?"

**🤖 AI Agent:**
> Your 10kg dog needs approximately 250ml of supplemental water daily. The high temperature and dry food increase the requirement.

---

**👤 You:**
> "What are the signs of dehydration for a cat in hot weather?"

**🤖 AI Agent:**
> In high temperatures, you should monitor for lethargy and changes in skin elasticity.

---

**👤 You:**
> "How much moisture is in wet food?"

**🤖 AI Agent:**
> Wet food provides a high percentage of hydration, significantly reducing the need for supplemental drinking water.


## ❓ FAQ

**Q: How does food type affect water needs?**
Different foods have different moisture levels. Dry food requires more supplemental drinking, while wet food provides significant inherent hydration.

**Q: Can I use this for both dogs and cats?**
Yes, the `calculate_daily_intake` tool supports both dog and cat species with specific metabolic baselines.

**Q: What should I look for if my pet is at risk?**
You can use `check_dehydration_indicators` to identify specific signs like changes in skin elasticity or lethargy based on current environmental heat.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-water-intake-calculator](https://vinkius.com/mcp/pet-water-intake-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Water Intake Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pet-water-intake-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Water Intake Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-water-intake-calculator": {
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
