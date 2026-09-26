# Severe Weather Readiness Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/severe-weather-readiness-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [emergency-management](../categories/emergency-management.md)

Transforms weather alerts and household data into prioritized readiness plans and execution roadmaps.

## Description
This MCP server provides critical decision support during extreme weather events. By synthesizing forecast alerts, property details, household schedules, and official mandates, it generates a chronological countdown plan. Use `generate_readiness_plan` to create a full response roadmap, `analyze_supply_shortfalls` to check food and water sufficiency, `compose_cancellation_templates` for urgent commitment cancellations, and `evaluate_evacuation_feasibility` to determine if safe movement is possible based on transport and official guidance.


## Available Tools (4)
- **analyze_supply_shortfalls**: Evaluates if current household supplies are sufficient for the expected duration
- **compose_cancellation_templates**: Generates ready-to-send messages for canceling commitments
- **evaluate_evacuation_feasibility**: Determines if the household can safely move to a secondary location
- **generate_readiness_plan**: Synthesizes all inputs into a comprehensive chronological response plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Severe Weather Readiness Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a readiness plan for a hurricane warning with the following alerts: [{"severity": "Warning", "expectedImpactTime": "2024-10-12T14:00:00Z", "eventType": "Hurricane"}] and my current supplies: {"water": "10L", "food": "5kg"}."

**🤖 AI Agent:**
> Immediate Action: Secure all loose outdoor items and move to the designated shelter location. Preparatory Action: Check water levels and ensure the first aid kit is accessible. Your current water supply is sufficient for the next 24 hours.

---

**👤 You:**
> "I need to cancel my work meeting due to a severe weather watch. The meeting is 'Project Sync' and the contact type is 'Professional'."

**🤖 AI Agent:**
> Dear Team, due to the current severe weather watch, I will be unable to attend the 'Project Sync' meeting. I will provide updates as soon as it is safe to do so.

---

**👤 You:**
> "Is it safe to evacuate? My fuel is 50%, my vehicle is functional, and there is currently a 'Shelter in Place' order."

**🤖 AI Agent:**
> No, evacuation is not feasible at this time because a 'Shelter in Place' order is currently active.


## ❓ FAQ

**Q: How does the server handle conflicting instructions?**
Official instructions from local government or emergency services always take precedence over user-defined triggers.

**Q: Can I use this to check if I have enough water for a storm?**
Yes, you can use the `analyze_supply_shortfalls` tool to evaluate if your current inventory is sufficient for the expected event duration.

**Q: What information is needed to generate a full plan?**
To use `generate_readiness_plan`, you should provide forecast alerts, property facts, household schedules, official instructions, user triggers, supply status, and transport status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/severe-weather-readiness-plan](https://vinkius.com/en/ai-agent-connect/severe-weather-readiness-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Severe Weather Readiness Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `severe-weather-readiness-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Severe Weather Readiness Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "severe-weather-readiness-plan": {
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
