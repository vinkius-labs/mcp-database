# Pet Event Attendance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-event-attendance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [event-management](../categories/event-management.md)

Track and analyze pet attendance and RSVP status for events.

## Description
This MCP server provides tools to manage pet event logistics by reconciling RSVP lists with actual attendance. Use `get_rsvp_summary` to view human RSVP counts, `calculate_pet_attendance` to find the expected number of pets, `check_capacity_status` to monitor remaining animal slots, and `get_attendance_metrics` to calculate no-show rates and participation percentages.


## Available Tools (4)
- **calculate_pet_attendance**: Calculates the total count of pets expected based on confirmed RSVPs
- **check_capacity_status**: Determines if the event has reached its maximum pet capacity
- **get_attendance_metrics**: Compares expected attendance against actual arrival data to calculate participation metrics
- **get_rsvp_summary**: Provides a high-level overview of the current RSVP status for an event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Event Attendance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many pets are expected to attend event ID 123?"

**🤖 AI Agent:**
> There are 15 pets expected to attend event 123 based on confirmed RSVPs.

---

**👤 You:**
> "Is event 456 at capacity?"

**🤖 AI Agent:**
> No, event 456 is not at capacity. There are 5 slots remaining.

---

**👤 You:**
> "What was the attendance percentage for event 789 if 20 pets were expected and 18 arrived?"

**🤖 AI Agent:**
> The attendance percentage for event 789 is 90%.


## ❓ FAQ

**Q: How do I check if my event is full?**
You can use the `check_capacity_status` tool to determine if the event has reached its maximum pet capacity and see how many slots remain.

**Q: Does this tool include pets from pending RSVPs?**
No, the `calculate_pet_attendance` tool only includes pets associated with human RSVPs that have a 'Confirmed' status.

**Q: How can I see the total number of human responses?**
Use the `get_rsvp_summary` tool to get a high-level overview, including total human RSVPs, confirmed, and pending counts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-event-attendance](https://vinkius.com/en/ai-agent-connect/pet-event-attendance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Event Attendance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-event-attendance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Event Attendance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-event-attendance": {
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
