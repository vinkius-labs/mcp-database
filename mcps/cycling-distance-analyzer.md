# Cycling Distance Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cycling-distance-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fitness](../categories/fitness.md)

Aggregate and analyze cumulative distance from cycling segments.

## Description
This MCP server provides tools to process cycling activity data. It allows AI agents to calculate total distance, identify the longest segment, find average lengths, and retrieve comprehensive distance statistics using `get_distance_statistics` and other specialized tools.


## Available Tools (4)
- **calculate_average_segment_length**: Calculate the average length of segments
- **calculate_total_distance**: Calculate the total distance covered across all provided segments
- **find_longest_segment**: Find the longest segment in a collection
- **get_distance_statistics**: Get high-level metrics for cycling segments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cycling Distance Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total distance of my segments: 5.2, 10.5, and 3.3?"

**🤖 AI Agent:**
> The total distance covered is 19.0.

---

**👤 You:**
> "Which segment was the longest among 12.4, 45.2, and 22.1?"

**🤖 AI Agent:**
> The longest segment is 45.2.

---

**👤 You:**
> "Give me the statistics for these segments: 10, 20, 30, 40."

**🤖 AI Agent:**
> Total distance: 100, Average: 25, Max: 40, Count: 4.


## ❓ FAQ

**Q: How can I get a summary of all my rides?**
You can use the `get_distance_statistics` tool to receive a summary including total distance, average length, maximum distance, and the total number of segments.

**Q: Can I find my longest ride segment?**
Yes, the `find_longest_segment` tool identifies the largest distance value within your provided list of segments.

**Q: What units should I use for segment lengths?**
You can use any consistent unit like kilometers or miles, as long as all segments in a single request use the same unit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cycling-distance-analyzer](https://vinkius.com/en/ai-agent-connect/cycling-distance-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cycling Distance Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cycling-distance-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cycling Distance Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cycling-distance-analyzer": {
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
