# Pet Walk Distance Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-walk-distance-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Track and analyze cumulative and average walking distances for pets.

## Description
This MCP server provides tools to monitor pet activity by calculating total distance traveled, average distance per walk, and detailed walk history within specific timeframes. Use `get_pet_total_distance` to find cumulative activity, `get_pet_average_walk_distance` for typical walk lengths, `get_walks_in_period` to list specific events, and `get_period_stats` for summary statistics over a defined date range.


## Available Tools (4)
- **get_period_stats**: Calculate summary statistics (total and average) for a pet within a specific timeframe
- **get_pet_average_walk_distance**: What is the typical distance covered during a single walk for this pet?
- **get_pet_total_distance**: How much total distance has a specific pet traveled?
- **get_walks_in_period**: List all individual walk events within a specific timeframe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Walk Distance Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much total distance has pet 'buddy-123' traveled?"

**🤖 AI Agent:**
> Buddy-123 has traveled a total distance of 45.5 kilometers over 12 walks.

---

**👤 You:**
> "What was the average walk distance for pet 'fluffy-456'?"

**🤖 AI Agent:**
> The average distance covered during a single walk for Fluffy-456 is 2.3 kilometers.

---

**👤 You:**
> "Give me the stats for pet 'rover-789' between 2024-01-01 and 2024-01-31."

**🤖 AI Agent:**
> In January 2024, Rover-789 completed 8 walks with a total distance of 18.4 kilometers and an average distance of 2.3 kilometers per walk.


## ❓ FAQ

**Q: How can I see the total distance my pet has walked?**
You can use the `get_pet_total_distance` tool by providing the unique pet ID.

**Q: Can I filter walk data by a specific date range?**
Yes, the `get_walks_in_period` and `get_period_stats` tools allow you to filter activity using start and end dates in ISO 8601 format.

**Q: What information is included in the period statistics?**
The `get_period_stats` tool returns the total distance, average distance, and the total number of walks recorded within the specified timeframe.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-walk-distance-tracker](https://vinkius.com/en/ai-agent-connect/pet-walk-distance-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Walk Distance Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-walk-distance-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Walk Distance Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-walk-distance-tracker": {
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
