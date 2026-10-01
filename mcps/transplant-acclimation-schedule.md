# Transplant Acclimation Schedule MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/transplant-acclimation-schedule)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Generate precise outdoor hardening schedules for plants.

## Description
This MCP server provides tools to manage the hardening process for indoor-grown plants. Use `generate_hardening_schedule` to create a day-by-day exposure plan, `validate_weather_impact` to check if current conditions require shade, `calculate_acclimation_status` to track progress toward the planting date, and `get_exposure_summary` for cumulative metrics.


## Available Tools (4)
- **calculate_acclimation_status**: Calculates the current progress of a plant's hardening relative to the target goal
- **generate_hardening_schedule**: Generates a day-by-day schedule of exposure requirements leading up to the planting date
- **get_exposure_summary**: Provides a summary of the total cumulative exposure requirements for a given period
- **validate_weather_impact**: Determines if the current weather conditions allow the hardening process to proceed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Transplant Acclimation Schedule** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a hardening schedule starting 2024-05-01, planting on 2024-05-15, with a 1-hour daily increment, 6 hours max sun, and 4 hours of shade."

**🤖 AI Agent:**
> The schedule for your plants from 2024-05-01 to 2024-05-15 is ready. It starts with minimal exposure and increases by 1 hour each day until reaching the 6-hour limit.

---

**👤 You:**
> "It is 32 degrees Celsius and windy. Should I protect my plants?"

**🤖 AI Agent:**
> The weather conditions are restricted. You should increase shade or bring your plants indoors to prevent damage.

---

**👤 You:**
> "How much progress have I made since May 1st if my planting date is May 15th?"

**🤖 AI Agent:**
> You have completed 45% of the required acclimation process, with 7 days remaining until the planting date.


## ❓ FAQ

**Q: What is plant hardening?**
Hardening is the process of gradually exposing indoor plants to outdoor conditions to prevent shock during transplanting.

**Q: How do I know if I should provide shade?**
You can use the `validate_weather_impact` tool to determine if current temperatures or wind speeds require you to increase shade or bring plants indoors.

**Q: Can I track my progress?**
Yes, the `calculate_acclimation_status` tool provides a percentage of completion and the number of days remaining until your target planting date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/transplant-acclimation-schedule](https://vinkius.com/en/ai-agent-connect/transplant-acclimation-schedule)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Transplant Acclimation Schedule** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `transplant-acclimation-schedule` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Transplant Acclimation Schedule** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "transplant-acclimation-schedule": {
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
