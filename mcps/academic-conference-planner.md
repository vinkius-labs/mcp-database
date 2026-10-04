# Academic Conference Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/academic-conference-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage conference schedules, registration fees, travel logistics, and networking windows.

## Description
This MCP server provides a complete toolkit for organizing academic conferences. It allows AI agents to `plan_session_schedule` for specific tracks, `calculate_registration_fees` based on participant roles, `verify_travel_alignment` to ensure attendees arrive in time for sessions, and `get_networking_opportunities` to identify social breaks.


## Available Tools (4)
- **plan_session_schedule**: Construct a logical sequence of academic sessions within a specific track
- **verify_travel_alignment**: Ensure a participant's travel and lodging details allow them to attend their scheduled sessions
- **calculate_registration_fees**: Determine the cost for an attendee based on their professional status and timing
- **get_networking_opportunities**: Identify available time slots dedicated to non-academic interaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Academic Conference Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a schedule for the 'AI Ethics' track with 3 sessions, each 60 minutes long and having 2 presentations per session."

**🤖 AI Agent:**
> The 'AI Ethics' track schedule has been created with 3 sessions of 60 minutes each, totaling 180 minutes of programming.

---

**👤 You:**
> "What is the fee for a Student registering during the Early Bird period?"

**🤖 AI Agent:**
> The registration fee for a Student with Early Bird status is $50.00.

---

**👤 You:**
> "Will a participant arriving on 2025-05-10T08:00:00Z be able to attend a session starting at 2025-05-10T11:00:00Z if their hotel check-in is at 2025-05-10T09:00:00Z?"

**🤖 AI Agent:**
> Yes, the travel alignment is feasible with a sufficient buffer before the first session.


## ❓ FAQ

**Q: How can I schedule a new track?**
You can use the `plan_session_schedule` tool to define the number of sessions and presentations for a specific track.

**Q: Can I check if a speaker's travel is feasible?**
Yes, use `verify_travel_alignment` to check if arrival and hotel check-in times allow for a sufficient buffer before the first session.

**Q: How are registration fees calculated?**
Fees are determined by the `calculate_registration_fees` tool, which considers the participant's role and early bird status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/academic-conference-planner](https://vinkius.com/en/ai-agent-connect/academic-conference-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Academic Conference Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `academic-conference-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Academic Conference Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "academic-conference-planner": {
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
