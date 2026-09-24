# Accessible Commute Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-commute-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates structured weekly transit schedules and contingency protocols based on specific mobility requirements.

## Description
This MCP server provides specialized planning tools for individuals with specific mobility needs. It connects AI agents to transit logistics by providing tools like `get_weekly_commute_plan` to build optimized itineraries, `get_booking_and_contact_actions` for logistical preparation, `get_backup_arrangements` for contingency routing, and `get_disruption_checklist` for immediate logistical response during transit interruptions. The service ensures all routes respect non-negotiable constraints such as mobility equipment and transfer limits.


## Available Tools (4)
- **get_backup_arrangements**: Provides secondary route options in case the primary plan is interrupted
- **get_booking_and_contact_actions**: Identifies the necessary logistical steps to finalize or prepare for the chosen commute
- **get_disruption_checklist**: Provides a logistical checklist for the user to follow when a disruption occurs
- **get_weekly_commute_plan**: Generates a full weekly schedule of optimized routes based on the user's specific constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Commute Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a weekly commute plan for a user with a power wheelchair who needs to arrive at work by 9:00 AM and prefers no more than 1 transfer."

**🤖 AI Agent:**
> Your weekly schedule is ready. Monday through Friday, you will depart at 8:15 AM via the accessible shuttle, arriving at 8:50 AM with 0 transfers.

---

**👤 You:**
> "What should I do if my bus is delayed and I have a service animal?"

**🤖 AI Agent:**
> Follow these logistical steps: 1. Check the secondary transit app for real-time updates. 2. Locate the nearest accessible station exit. 3. Contact the transit assistance desk.

---

**👤 You:**
> "What actions do I need to take to prepare for my commute tomorrow?"

**🤖 AI Agent:**
> You need to complete the following: 1. Book the accessible taxi via the mobile app. 2. Notify the station staff for boarding assistance.


## ❓ FAQ

**Q: How does the tool handle mobility equipment?**
The `get_weekly_commute_plan` tool uses your specified mobility equipment to filter for routes that meet all physical requirements, such as ramp access or door width.

**Q: Can I get backup routes if my primary plan is interrupted?**
Yes, you can use `get_backup_arrangements` to generate secondary route options that still respect your mobility constraints and departure windows.

**Q: Does this provide medical advice during disruptions?**
No. The `get_disruption_checklist` tool provides purely logistical steps, such as locating exits or checking secondary apps, and does not provide medical or physical health advice.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-commute-planner](https://vinkius.com/en/ai-agent-connect/accessible-commute-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Commute Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-commute-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Commute Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-commute-planner": {
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
