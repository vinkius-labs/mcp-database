# Photo Session Timekeeper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/photo-session-timekeeper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates precise photography session timelines including setups, shots, and breaks.

## Description
Photo Session Timekeeper helps photography production managers build accurate schedules. By providing start and end times, subjects, shot durations, setup times, and planned breaks, you can use `calculate_session_timeline` to generate a complete chronological list of events. You can also use `validate_session_capacity` to ensure a shoot plan fits within the available window, `get_subject_load_analysis` to identify heavy workloads, and `find_earliest_break_slot` to locate optimal break times.


## Available Tools (4)
- **find_earliest_break_slot**: Suggests the earliest possible time a break can occur based on the current scheduled sequence
- **calculate_session_timeline**: Generates a complete chronological list of scheduled events and identifies remaining unscheduled time
- **get_subject_load_analysis**: Analyzes how much time is allocated to each subject to identify heavy subjects
- **validate_session_capacity**: Determines if a proposed list of shots and breaks can physically fit within a specific timeframe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Photo Session Timekeeper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a timeline for a shoot starting at 2024-10-01T09:00:00Z and ending at 2024-10-01T12:00:00Z. Subjects are 'Model A' and 'Model B'. Shot durations are 30 and 45 minutes. Setup times are 10 and 15 minutes. There is one 20-minute break."

**🤖 AI Agent:**
> The session timeline is as follows: 09:00 - 09:10 Setup for Model A, 09:10 - 09:40 Shot of Model A, 09:40 - 10:00 Break, 10:00 - 10:15 Setup for Model B, 10:15 - 11:00 Shot of Model B. Total unscheduled time remaining: 60 minutes.

---

**👤 You:**
> "Check if I can fit two 60-minute shots with 15-minute setups and a 30-minute break between 10:00 AM and 12:00 PM."

**🤖 AI Agent:**
> Yes, the total required time is 180 minutes, which fits within the 120-minute window? Wait, the total required time is 15+60+30+15+60 = 180 minutes. The session is only 120 minutes. The plan is not feasible.

---

**👤 You:**
> "Analyze the workload for subjects: 'Portrait 1' (45m shot, 10m setup) and 'Portrait 2' (30m shot, 20m setup)."

**🤖 AI Agent:**
> Portrait 1 has a total load of 55 minutes, and Portrait 2 has a total load of 50 minutes.


## ❓ FAQ

**Q: How do I know if my shoot plan is feasible?**
You can use the `validate_session_capacity` tool to check if your proposed shots, setups, and breaks fit within your specified start and end times.

**Q: Can I see how much time is allocated to each subject?**
Yes, the `get_subject_load_analysis` tool provides a breakdown of the total time footprint (setup plus shot duration) for every subject.

**Q: What happens to the extra time in a session?**
Any remaining time after all scheduled shots, setups, and breaks is identified as unscheduled duration by the `calculate_session_timeline` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/photo-session-timekeeper](https://vinkius.com/en/ai-agent-connect/photo-session-timekeeper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Photo Session Timekeeper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `photo-session-timekeeper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Photo Session Timekeeper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "photo-session-timekeeper": {
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
