# Swimming Distance Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/swimming-distance-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate and aggregate swimming distances across sessions.

## Description
This MCP server provides tools to manage swimming training data. You can use `calculate_session_distance` to find the total distance of a single swim, `aggregate_multiple_sessions` to sum distances from various workouts, `validate_pool_standard` to check if a pool size is a recognized international standard, and `convert_distance` to switch between meters and yards.


## Available Tools (4)
- **aggregate_multiple_sessions**: Sums the total distance across multiple different swimming sessions
- **calculate_session_distance**: Calculates the total distance covered in a single swimming session
- **convert_distance**: Converts a distance from one unit to another
- **validate_pool_standard**: Verifies if a provided pool length matches recognized international swimming standards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swimming Distance Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How far did I swim if I did 20 lengths in a 25 meter pool?"

**🤖 AI Agent:**
> You swam a total of 500 meters.

---

**👤 You:**
> "Is a 50 yard pool a standard size?"

**🤖 AI Agent:**
> No, 50 yards is not a recognized standard pool length.

---

**👤 You:**
> "Convert 100 meters to yards."

**🤖 AI Agent:**
> 100 meters is approximately 109.36 yards.


## ❓ FAQ

**Q: How do I calculate the distance of one swim?**
You can use the `calculate_session_distance` tool by providing the pool length, the number of lengths completed, and the unit used.

**Q: Can I sum up multiple training sessions at once?**
Yes, the `aggregate_multiple_sessions` tool allows you to provide a list of different sessions to get a grand total distance.

**Q: Does it support both meters and yards?**
Yes, all tools support both meters and yards, and you can use `convert_distance` to switch between them.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/swimming-distance-calculator](https://vinkius.com/en/ai-agent-connect/swimming-distance-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Swimming Distance Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `swimming-distance-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Swimming Distance Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "swimming-distance-calculator": {
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
