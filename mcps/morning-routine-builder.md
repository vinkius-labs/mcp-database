# Morning Routine Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/morning-routine-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A backward scheduling engine for precise morning timelines.

## Description
Morning Routine Builder uses backward scheduling logic to calculate the exact start times for your morning activities. By starting from your fixed departure time and working backward, it accounts for task durations, sequential dependencies, and safety buffers. Use `generate_routine` to create a full timeline, `validate_dependencies` to ensure your schedule is logically sound, and `calculate_buffer_impact` to see how much extra sleep you can get by adjusting your buffer or removing optional tasks.


## Available Tools (4)
- **calculate_buffer_impact**: Determines how much extra sleep or free time is gained by adjusting the buffer or removing optional tasks
- **get_task_metadata**: Retrieves the specific properties and requirements of a single task within a defined routine
- **validate_dependencies**: Checks if a proposed set of task dependencies is logically possible and free of conflicts
- **generate_routine**: Calculates the complete morning timeline based on a target departure and a list of tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Morning Routine Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a routine where I need to leave at 08:00. Tasks: Shower (15m), Breakfast (20m, depends on Shower), Get Dressed (10m, depends on Shower). Include a 5 minute buffer."

**🤖 AI Agent:**
> Your morning timeline is ready. To leave at 08:00 with a 5-minute buffer, you should wake up at 07:10. Shower starts at 07:10, Breakfast starts at 07:25, and Getting Dressed starts at 07:45.

---

**👤 You:**
> "How much extra sleep can I get if I remove my 10-minute buffer?"

**🤖 AI Agent:**
> By removing the 10-minute buffer, you will gain exactly 10 minutes of extra sleep.

---

**👤 You:**
> "What are the details for the 'Shower' task?"

**🤖 AI Agent:**
> The Shower task has a duration of 15 minutes and is a mandatory task.


## ❓ FAQ

**Q: How does the scheduling work?**
The engine uses backward scheduling. It starts at your departure time and subtracts the duration of each task and any required buffers to find the latest possible wake-up time.

**Q: Can I include optional tasks?**
Yes, you can use the `includeOptional` parameter in `generate_routine` to decide whether to include tasks marked as optional in your timeline.

**Q: How do I check for errors in my schedule?**
You can use the `validate_dependencies` tool to check if your task dependencies are logically possible and free of circular conflicts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/morning-routine-builder](https://vinkius.com/en/ai-agent-connect/morning-routine-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Morning Routine Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `morning-routine-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Morning Routine Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "morning-routine-builder": {
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
