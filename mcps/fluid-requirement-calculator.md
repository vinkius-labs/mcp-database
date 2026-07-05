# Fluid Requirement Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fluid-requirement-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate personalized daily fluid intake needs based on weight, age, and environmental factors.

## Description
This MCP server provides a specialized calculation engine to determine your total daily water requirements. By using tools like `calculate_baseline_requirement`, you can establish a physiological baseline based on weight and age (pediatric or adult). The engine then layers adjustments via `calculate_environmental_modifiers` for factors such as fever, exercise duration, altitude, and breastfeeding. Finally, `get_final_daily_target` orchestrates the full calculation, ensuring your recommendation meets the 2.5L safety threshold for kidney stone prevention.


## Available Tools (3)
- **calculate_baseline_requirement**: Calculate the baseline fluid requirement
- **calculate_environmental_modifiers**: Calculate environmental fluid adjustments
- **get_final_daily_target**: 5L).

Calculate the total daily fluid target


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fluid Requirement Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my daily water target if I weigh 70kg, am an adult, and just finished a 60-minute run?"

**🤖 AI Agent:**
> Based on your weight of 70kg and 60 minutes of exercise, your recommended daily fluid intake is 3500ml.

---

**👤 You:**
> "Calculate the baseline requirement for a 15kg child."

**🤖 AI Agent:**
> The baseline fluid requirement for a 15kg pediatric patient is 1000ml.

---

**👤 You:**
> "How much extra water do I need if my temperature is 39C and I am at 2500m altitude?"

**🤖 AI Agent:**
> The environmental modifiers add an additional volume to your baseline to compensate for fever and high altitude.


## ❓ FAQ

**Q: How does the baseline calculation work?**
The `calculate_baseline_requirement` tool uses the Holliday-Segar method for pediatric patients and a standard milliliters per kilogram ratio for adults.

**Q: What environmental factors are considered?**
The engine accounts for fever (temperature above 38C), physical activity duration, altitude elevation, and breastfeeding status.

**Q: Is there a minimum fluid recommendation?**
Yes, the `get_final_daily_target` tool enforces a safety floor of 2.5 liters per day to assist in kidney stone prevention.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fluid-requirement-calculator](https://vinkius.com/mcp/fluid-requirement-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fluid Requirement Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fluid-requirement-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fluid Requirement Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fluid-requirement-calculator": {
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
