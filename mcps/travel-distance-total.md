# Travel Distance Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/travel-distance-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Calculate cumulative, average, and extreme travel leg distances.

## Description
This MCP server provides tools to analyze travel segments. Use `calculate_total_distance` to sum multiple legs, `get_average_leg_distance` for the mean, `find_longest_leg` to identify the largest segment, and `validate_distance_segments` to ensure all distances are non-negative.


## Available Tools (4)
- **calculate_total_distance**: Adds supplied travel-leg distances and returns total distance
- **find_longest_leg**: Identifies the single longest segment within a journey
- **get_average_leg_distance**: Determines the mean distance of all travel segments
- **validate_distance_segments**: Checks if a collection of distances adheres to physical and logical constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Travel Distance Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total distance for legs of 10, 25, and 5 miles?"

**🤖 AI Agent:**
> The total distance is 40 miles.

---

**👤 You:**
> "What is the average distance of 100, 200, and 300 km?"

**🤖 AI Agent:**
> The average distance is 200 km.

---

**👤 You:**
> "Which is the longest leg in a trip with distances 5, 50, and 12?"

**🤖 AI Agent:**
> The longest leg is 50.


## ❓ FAQ

**Q: How do I sum multiple travel distances?**
You can use the `calculate_total_distance` tool by providing an array of distances.

**Q: Can I check if my distance data is valid?**
Yes, the `validate_distance_segments` tool checks if all provided distances are non-negative numbers.

**Q: How can I find the longest part of my trip?**
Use the `find_longest_leg` tool to identify the maximum distance in your list of segments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/travel-distance-total](https://vinkius.com/en/ai-agent-connect/travel-distance-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Travel Distance Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `travel-distance-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Travel Distance Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "travel-distance-total": {
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
