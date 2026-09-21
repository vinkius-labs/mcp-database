# Hydrotherapy Tub Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hydrotherapy-tub-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculates optimal hydrotherapy jet settings, duration, and treatment schedules.

## Description
This MCP server provides precise hydrotherapy configurations based on physiological needs. Use `get_jet_settings` to determine pressure and movement patterns for specific body parts, `get_treatment_schedule` to plan recovery periods, `validate_thermal_safety` to ensure temperature compliance, and `get_movement_pattern_details` to understand specific water flow benefits.


## Available Tools (4)
- **get_treatment_schedule**: Determines the recommended frequency and duration of treatments over a set period
- **get_jet_settings**: Calculates the specific mechanical configuration for a single hydrotherapy session
- **get_movement_pattern_details**: Provides a description of the intended water movement for a given configuration
- **validate_thermal_safety**: Checks if a specific temperature and target area combination poses a risk of skin irritation or thermal injury


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hydrotherapy Tub Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What jet settings should I use for lower back muscle spasms at 38 degrees Celsius?"

**🤖 AI Agent:**
> For lower back muscle spasms at 38°C, use a pulsating movement pattern with a jet pressure of 45 kPa for a duration of 15 minutes.

---

**👤 You:**
> "Is 41 degrees Celsius safe for my neck?"

**🤖 AI Agent:**
> No, 41°C is considered high for the neck area and may pose a risk of skin irritation.

---

**👤 You:**
> "What is a good treatment schedule for chronic stiffness?"

**🤖 AI Agent:**
> For chronic stiffness with medium intensity, it is recommended to have 3 sessions per week for 4 weeks.


## ❓ FAQ

**Q: How do I know if the water temperature is safe for my treatment?**
You can use the `validate_thermal_safety` tool to check if a specific temperature is safe for your target area.

**Q: Can I plan a long-term recovery plan?**
Yes, the `get_treatment_schedule` tool provides recommended sessions per week and total duration for various conditions.

**Q: What information do I need to get jet settings?**
To use `get_jet_settings`, you need to provide the target area, the condition being treated, and the water temperature.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hydrotherapy-tub-calculator](https://vinkius.com/en/ai-agent-connect/hydrotherapy-tub-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hydrotherapy Tub Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hydrotherapy-tub-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hydrotherapy Tub Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hydrotherapy-tub-calculator": {
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
