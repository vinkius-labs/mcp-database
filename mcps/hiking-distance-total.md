# Hiking Distance Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hiking-distance-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate and manage cumulative hiking distances from individual trail segments.

## Description
This MCP server provides tools to manage hiking data. You can use `get_total_distance` to sum multiple segments, `get_segment_details` to retrieve specific trail information, `validate_segment_list` to ensure segments are valid, and `compare_segments` to find the difference between two trails.


## Available Tools (4)
- **get_segment_details**: Get the name and length of a specific hiking segment
- **compare_segments**: Compare the lengths of two hiking segments
- **get_total_distance**: Calculate the total distance covered by a list of segment IDs
- **validate_segment_list**: Validate if a list of segment IDs are all valid and have positive lengths


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hiking Distance Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total distance for segments seg-123 and seg-456?"

**🤖 AI Agent:**
> The total distance for those segments is 15.5 kilometers.

---

**👤 You:**
> "How long is the segment known as seg-789?"

**🤖 AI Agent:**
> The segment seg-789 is 5.2 kilometers long.

---

**👤 You:**
> "Which is longer: seg-111 or seg-222?"

**🤖 AI Agent:**
> seg-222 is longer by 2.4 kilometers.


## ❓ FAQ

**Q: How do I calculate the total distance of my hike?**
You can use the `get_total_distance` tool by providing a list of segment IDs.

**Q: Can I check if my selected segments are valid?**
Yes, use the `validate_segment_list` tool to verify that all segments exist and have positive lengths.

**Q: How can I compare two different trails?**
Use the `compare_segments` tool to find the absolute difference in length between two specific segments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hiking-distance-total](https://vinkius.com/en/ai-agent-connect/hiking-distance-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hiking Distance Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hiking-distance-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hiking Distance Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hiking-distance-total": {
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
