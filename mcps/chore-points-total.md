# Chore Points Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/chore-points-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage and track reward points earned through completed household chores.

## Description
This MCP server connects AI agents to a household reward system. It allows users to check their current point balance using `get_user_balance`, view a list of tasks available to perform via `list_available_chores`, claim points for finished tasks with `complete_chore`, and review their activity log through `get_chore_history`. It is designed to encourage consistent participation in household responsibilities by providing a clear, automated way to track progress.


## Available Tools (4)
- **complete_chore**: Complete chore
- **get_chore_history**: Get history
- **get_user_balance**: Get user balance
- **list_available_chores**: List chores


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chore Points Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many points does user_123 have?"

**🤖 AI Agent:**
> User user_123 currently has 150 reward points.

---

**👤 You:**
> "What chores can I do in the Kitchen?"

**🤖 AI Agent:**
> In the Kitchen, you can complete 'Wash Dishes' (10 points) or 'Clean Microwave' (15 points).

---

**👤 You:**
> "I just finished the 'Vacuum Living Room' chore. My user ID is user_456 and the chore ID is chore_789."

**🤖 AI Agent:**
> Success! You earned 20 points. Your new balance is 85 points.


## ❓ FAQ

**Q: How do I see how many points I have?**
You can use the `get_user_balance` tool by providing your unique user ID to see your current total.

**Q: Can I see what tasks are available to do?**
Yes, use the `list_available_chores` tool to see all tasks and the points they are worth. You can also filter by category.

**Q: How do I claim my points after finishing a chore?**
Once a task is finished, use the `complete_chore` tool with your user ID and the specific chore ID to add the points to your balance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/chore-points-total](https://vinkius.com/en/ai-agent-connect/chore-points-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chore Points Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chore-points-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chore Points Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chore-points-total": {
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
