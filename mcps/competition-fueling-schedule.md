# Competition Fueling Schedule MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/competition-fueling-schedule)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Generates precise nutrition and hydration timelines for athletes.

## Description
This MCP server provides professional nutrition planning for athletes. It uses specialized tools like `generate_fueling_timeline` to create chronological schedules, `calculate_carb_loading_protocol` for glycogen saturation, `get_intra_event_strategy` for hourly fueling, and `validate_event_timing` to adjust windows for morning or afternoon starts. It ensures metabolic readiness through precise carbohydrate and hydration planning.


## Available Tools (4)
- **calculate_carb_loading_protocol**: Determines specific carbohydrate intake requirements for the days leading up to the event
- **generate_fueling_timeline**: Generates a comprehensive, chronological nutrition and hydration schedule for an athlete
- **get_intra_event_strategy**: Calculates specific hourly fueling and hydration requirements during the competition
- **validate_event_timing**: Adjusts fueling windows based on whether an event occurs in the morning or afternoon


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Competition Fueling Schedule** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a fueling timeline for a 120-minute endurance race starting at 2024-07-04T08:00:00Z with 5g of carbs per kg."

**🤖 AI Agent:**
> Your schedule includes a carbohydrate loading phase starting 3 days prior, a pre-event meal at 05:00 AM, and hourly fueling of 60g of carbohydrates during the race.

---

**👤 You:**
> "How much should I load carbs for a 70kg athlete for 3 days?"

**🤖 AI Agent:**
> For a 70kg athlete loading for 3 days at 10g/kg, you will need a total of 2100g of carbohydrates.

---

**👤 You:**
> "What is my intra-event strategy for a 60-minute race with 1g/min carb target and 1L/hr sweat rate?"

**🤖 AI Agent:**
> You need to consume 60g of carbohydrates and 1000ml of fluid per hour during the event.


## ❓ FAQ

**Q: How does the tool handle different event times?**
The `validate_event_timing` tool adjusts fueling windows based on whether the event starts in the morning or afternoon to optimize metabolic readiness.

**Q: Can I plan my carbohydrate loading phase?**
Yes, you can use `calculate_carb_loading_protocol` to determine the specific carbohydrate intake requirements for the days leading up to your competition.

**Q: Does it provide hydration advice?**
Yes, the `generate_fueling_timeline` tool includes a complete hydration schedule alongside nutrition timing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/competition-fueling-schedule](https://vinkius.com/en/ai-agent-connect/competition-fueling-schedule)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Competition Fueling Schedule** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `competition-fueling-schedule` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Competition Fueling Schedule** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "competition-fueling-schedule": {
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
