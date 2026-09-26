# Caregiver Routine Handoff MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/caregiver-routine-handoff)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates a unified, chronological daily guide for caregivers by synthesizing schedules, meals, and safety protocols.

## Description
This MCP server provides a single, linear timeline for caregivers to reduce cognitive load. By using `get_daily_guide`, caregivers receive a unified schedule that merges meals, activities, and comfort preferences into one chronological flow. It also provides direct access to critical safety data via `get_emergency_protocols` and dietary requirements through `get_dietary_profile`, ensuring all restrictions are integrated into the daily routine.


## Available Tools (4)
- **get_comfort_preferences**: Retrieves non-medical preferences used to ensure patient comfort and routine consistency
- **get_daily_guide**: Generates a complete, chronological timeline of events for a specific date
- **get_dietary_profile**: Retrieves a summary of all dietary requirements and restrictions for the individual
- **get_emergency_protocols**: Provides immediate access to contact information and escalation procedures


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Caregiver Routine Handoff** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you show me the daily schedule for 2024-12-25?"

**🤖 AI Agent:**
> Here is the daily guide for 2024-12-25: 08:00 - Breakfast (Low sodium meal), 10:00 - Morning Walk (Use mobility aid), 12:00 - Lunch (Soft foods only).

---

**👤 You:**
> "What are the emergency contact details for subject ID 123?"

**🤖 AI Agent:**
> The primary contact is Jane Doe (Relative) at 555-0199. Escalation steps: 1. Contact Jane, 2. Call emergency services.

---

**👤 You:**
> "What are the dietary restrictions for this patient?"

**🤖 AI Agent:**
> The patient has the following restrictions: Low sodium diet, no peanuts, and prefers soft foods.


## ❓ FAQ

**Q: How does the daily guide handle dietary restrictions?**
The `get_daily_guide` tool automatically integrates dietary restrictions from the `get_dietary_profile` into the relevant meal descriptions in the timeline.

**Q: Can I access emergency contacts quickly?**
Yes, you can use the `get_emergency_protocols` tool to immediately retrieve primary contacts and escalation steps.

**Q: What information is included in the daily guide?**
The guide includes a chronological timeline of activities, meal times, dietary restrictions, comfort preferences, and emergency protocols.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/caregiver-routine-handoff](https://vinkius.com/en/ai-agent-connect/caregiver-routine-handoff)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Caregiver Routine Handoff** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `caregiver-routine-handoff` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Caregiver Routine Handoff** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "caregiver-routine-handoff": {
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
