# Cycle Day Resolver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cycle-day-resolver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Identify specific tasks or states for any future date based on a repeating, variable-length sequence.

## Description
The Cycle Day Resolver MCP server acts as a temporal engine that calculates exactly what step to take on any given future date based on a variable-length cycle. By providing an ordered array of steps and an anchor start date, you can use tools like `get_step_for_date` to find specific tasks, `get_schedule_window` to forecast upcoming periods, or `find_next_occurrence` to locate the next instance of a particular event. It is ideal for managing recurring skincare routines, medication schedules, or any repeating operational loop.


## Available Tools (4)
- **analyze_cycle_composition**: Returns total length and step frequencies as JSON.

Provides a statistical overview of the cycle's structure and frequency
- **find_next_occurrence**: Searches forward in time to find the very next date a specific step will appear
- **get_schedule_window**: Returns a list of dates and steps.

Generates a complete chronological forecast of all steps within a specific time range
- **get_step_for_date**: Returns the resolved step name.

Identifies which specific step or task is scheduled for a particular target date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cycle Day Resolver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my skincare step for 2025-06-15 if my cycle ['Retinol', 'Exfoliant', 'Recovery'] started on 2025-01-01?"

**🤖 AI Agent:**
> On 2025-06-15, your scheduled step is Exfoliant.

---

**👤 You:**
> "Show me my schedule from 2025-07-01 to 2025-07-05 for the cycle ['Day', 'Night'] starting 2025-01-01."

**🤖 AI Agent:**
> 2025-07-01: Day, 2025-07-02: Night, 2025-07-03: Day, 2025-07-04: Night, 2025-07-05: Day.

---

**👤 You:**
> "When is the next time 'Exfoliant' occurs in my cycle ['Retinol', 'Exfoliant', 'Recovery'] starting 2025-01-01, searching from 2025-02-01?"

**🤖 AI Agent:**
> The next occurrence of Exfoliant is on 2025-02-02.


## ❓ FAQ

**Q: How does the cycle resolution logic work?**
The engine calculates the number of days elapsed between your anchor start date and the target date, then finds the remainder when divided by the total cycle length to identify the correct step.

**Q: Can I use this for skincare routines?**
Yes, you can provide a cycle array like ['Retinol', 'Exfoliant', 'Recovery'] and an anchor date to determine exactly which product to use on any future morning.

**Q: What happens if the target date is before the start date?**
The `get_step_for_date` tool will return an error stating that the target date must be equal to or later than the anchor date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cycle-day-resolver](https://vinkius.com/mcp/cycle-day-resolver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cycle Day Resolver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cycle-day-resolver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cycle Day Resolver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cycle-day-resolver": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
