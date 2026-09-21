# Embroidery Stitch Count Utility MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/embroidery-stitch-count-utility)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [manufacturing](../categories/manufacturing.md)

Calculate and aggregate stitch counts for embroidery production planning.

## Description
This MCP server provides specialized tools for embroidery production management. It allows users to retrieve specific metadata for individual designs using `get_design_details`, calculate cumulative workloads for production batches with `calculate_batch_total`, find complexity scaling factors via `get_complexity_multiplier`, and filter designs by density using `search_designs_by_density`. It acts as a bridge between design assets and production planning workflows.


## Available Tools (4)
- **calculate_batch_total**: 
- **get_complexity_multiplier**: 
- **get_design_details**: 
- **search_designs_by_density**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Embroidery Stitch Count Utility** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total stitch count for designs ID-101 and ID-102?"

**🤖 AI Agent:**
> The total stitch count for the requested designs is 15,450 stitches.

---

**👤 You:**
> "How many stitches are in design ID-505?"

**🤖 AI Agent:**
> Design ID-505 has a total stitch count of 8,200.

---

**👤 You:**
> "What is the multiplier for an Advanced complexity tier?"

**🤖 AI Agent:**
> The multiplier for the Advanced complexity tier is 1.5.


## ❓ FAQ

**Q: How can I estimate the total workload for a production run?**
You can use the `calculate_batch_total` tool by providing a list of design IDs to get the cumulative stitch count.

**Q: Can I find designs with specific density levels?**
Yes, the `search_designs_by_density` tool allows you to filter designs within a specified minimum and maximum density range.

**Q: What information is included in a design's details?**
Using `get_design_details` provides the design name, unique ID, total stitch count, complexity level, and density factor.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/embroidery-stitch-count-utility](https://vinkius.com/en/ai-agent-connect/embroidery-stitch-count-utility)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Embroidery Stitch Count Utility** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `embroidery-stitch-count-utility` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Embroidery Stitch Count Utility** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "embroidery-stitch-count-utility": {
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
