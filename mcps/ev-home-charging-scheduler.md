# EV Home Charging Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ev-home-charging-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate optimal EV charging schedules within off-peak electricity windows.

## Description
This MCP server provides specialized tools to optimize electric vehicle charging. It calculates precise charging windows based on available off-peak electricity periods, vehicle battery capacity, and charger power. Use `calculate_charging_window` to determine the best start and end times for a charge, or `get_energy_requirement` to find the exact kWh needed to reach a target state of charge. It also includes `validate_charger_capability` to ensure your hardware can meet your needs and `summarize_charging_efficiency` to account for energy losses during the process.


## Available Tools (4)
- **calculate_charging_window**: Determines the specific start and end times for a charging session and identifies if the target was met
- **get_energy_requirement**: Calculates the raw energy (kWh) needed to move from one SoC to another
- **summarize_charging_efficiency**: Provides a high-level summary of how much energy is lost to heat and conversion during the process
- **validate_charger_capability**: Checks if the hardware is physically capable of attempting the requested charge


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EV Home Charging Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a charging schedule for my EV. I have 40% charge, I want 80%, a 75kWh battery, a 7kW charger, 90% efficiency, and an off-peak window from 2024-05-01T01:00:00Z to 2024-05-01T06:00:00Z."

**🤖 AI Agent:**
> The optimal charging window is from 2024-05-01T01:00:00Z to 2024-05-01T06:00:00Z. Total energy delivered to battery: 31.5 kWh. Target met.

---

**👤 You:**
> "How much energy do I need to go from 20% to 90% on a 100kWh battery?"

**🤖 AI Agent:**
> You need 70 kWh to reach your target charge level.

---

**👤 You:**
> "Can a 3kW charger handle a 100kWh battery for a standard overnight charge?"

**🤖 AI Agent:**
> The charger is capable of providing meaningful charge within a standard overnight window.


## ❓ FAQ

**Q: How does the tool handle electricity costs?**
The tool uses the provided off-peak windows to schedule charging when electricity is cheapest, ensuring you maximize savings.

**Q: What happens if the charger is too slow to reach the target SoC?**
The `calculate_charging_window` tool will return the scheduled time and report the unmet energy in kWh that could not be delivered within the window.

**Q: Does this account for charging losses?**
Yes, you can provide an efficiency decimal to account for energy lost to heat and conversion during the charging process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ev-home-charging-scheduler](https://vinkius.com/en/ai-agent-connect/ev-home-charging-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EV Home Charging Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ev-home-charging-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EV Home Charging Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ev-home-charging-scheduler": {
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
