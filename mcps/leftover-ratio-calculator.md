# Leftover Ratio Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/leftover-ratio-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Minimize food waste by calculating optimal portions for events.

## Description
The Leftover Ratio Calculator is an estimation engine designed for event planners to determine the ideal quantities of food and beverages. By analyzing guest counts, meal types (such as casual lunch, formal dinner, or buffet), and appetite levels, it provides precise weights for main courses, sides, starches, and vegetables, alongside beverage requirements. Use tools like `calculate_main_course_portions` and `analyze_waste_risk` to optimize your event planning and mitigate food waste.


## Available Tools (4)
- **calculate_sides_and_starches**: Calculate required starch and vegetable amounts
- **analyze_waste_risk**: Analyze potential food waste risk
- **estimate_beverage_requirements**: Estimate required beverage amounts
- **calculate_main_course_portions**: Calculate required main course portions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Leftover Ratio Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much meat do I need for 50 people at a buffet with high appetite?"

**🤖 AI Agent:**
> For 50 guests at a buffet with a high appetite level, you will need approximately 12,500 grams of main course protein.

---

**👤 You:**
> "What is the risk of waste for a formal dinner with 100 guests?"

**🤖 AI Agent:**
> The waste risk level for a formal dinner with 100 guests is low, as structured service allows for better portion control.

---

**👤 You:**
> "How many liters of water should I prepare for a 3-hour casual lunch with 20 people?"

**🤖 AI Agent:**
> For a 3-hour event with 20 guests, you should prepare approximately 15 liters of beverages.


## ❓ FAQ

**Q: How do I calculate the amount of protein needed?**
Use the `calculate_main_course_portions` tool by providing the number of guests, the meal type (e.g., buffet), and the expected appetite level.

**Q: Can I estimate beverage needs for my event?**
Yes, the `estimate_beverage_requirements` tool calculates total liters and bottles required based on your guest count and event duration.

**Q: How does the tool help reduce food waste?**
The `analyze_waste_risk` tool identifies high-risk scenarios, such as large buffets with high appetite levels, and provides specific mitigation strategies to prevent leftovers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leftover-ratio-calculator](https://vinkius.com/mcp/leftover-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Leftover Ratio Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `leftover-ratio-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Leftover Ratio Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "leftover-ratio-calculator": {
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
