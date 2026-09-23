# Room Task Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/room-task-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and count completed tasks across different rooms.

## Description
This MCP server provides tools to manage and monitor task progress within a facility. You can use `list_all_rooms` to see all available spaces, `get_room_details` to check specific room metadata, and `get_room_task_counts` to get a summary of completed work across multiple rooms. It also includes `get_room_completion_rate` to calculate progress percentages.


## Available Tools (4)
- **get_room_details**: 
- **get_room_task_counts**: 
- **list_all_rooms**: 
- **get_room_completion_rate**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Room Task Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the rooms in the system."

**🤖 AI Agent:**
> The available rooms are: Kitchen, Living Room, Bedroom 1, and Office.

---

**👤 You:**
> "How many tasks are completed in the Kitchen and the Office?"

**🤖 AI Agent:**
> There are 5 completed tasks in the Kitchen and 3 completed tasks in the Office.

---

**👤 You:**
> "What is the completion rate for the Living Room?"

**🤖 AI Agent:**
> The completion rate for the Living Room is 75%.


## ❓ FAQ

**Q: How can I see all available rooms?**
You can use the `list_all_rooms` tool to retrieve a complete list of all rooms currently tracked in the system.

**Q: Can I check the progress of a specific room?**
Yes, use `get_room_completion_rate` to find the percentage of tasks completed in a specific room.

**Q: How do I get counts for multiple rooms at once?**
Use the `get_room_task_counts` tool and provide an array of room names to get the completed task counts for all of them.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/room-task-counter](https://vinkius.com/en/ai-agent-connect/room-task-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Room Task Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `room-task-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Room Task Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "room-task-counter": {
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
