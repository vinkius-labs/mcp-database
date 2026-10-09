# Embroidery Thread Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/embroidery-thread-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total thread length and required skeins for embroidery designs.

## Description
This MCP server provides precise calculations for embroidery production. Use `get_total_thread_requirement` to determine the total length of thread needed, including a configurable waste factor. Use `calculate_skein_count` to find out exactly how many full skeins must be purchased for a design. You can also use `get_material_efficiency_ratio` to see how much of a skein is utilized, or `validate_stitch_parameters` to ensure your input values are within realistic machine limits.


## Available Tools (4)
- **calculate_skein_count**: Determines how many full skeins of thread must be purchased
- **get_material_efficiency_ratio**: Evaluates how much of a purchased skein is utilized by a specific design
- **get_total_thread_requirement**: Calculates the total length of thread needed for a specific embroidery task
- **validate_stitch_parameters**: Checks if the provided stitch and length parameters are within realistic operational bounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Embroidery Thread Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much thread do I need for 5000 stitches if each stitch uses 2mm of thread and I want a 10% waste factor?"

**🤖 AI Agent:**
> You will need a total of 11000mm of thread (10000mm base + 1000mm waste).

---

**👤 You:**
> "I need 15000mm of thread and my skeins are 4000mm each. How many skeins do I need?"

**🤖 AI Agent:**
> You will need to purchase 4 skeins.

---

**👤 You:**
> "Is a stitch count of 1,000,000 and a length per stitch of 0.5mm realistic?"

**🤖 AI Agent:**
> Yes, these parameters are within realistic operational bounds.


## ❓ FAQ

**Q: How do I calculate the total thread needed?**
You can use the `get_total_thread_requirement` tool by providing the total stitch count, the length of thread used per stitch, and an optional waste percentage.

**Q: How many skeins should I buy?**
Use the `calculate_skein_count` tool. Provide the total required length (including waste) and the length of a single skein to get the minimum number of whole skeins required.

**Q: Can I account for thread waste?**
Yes, the `get_total_thread_requirement` tool includes a `wastePercentage` parameter to account for machine threading, starts, stops, and breakage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/embroidery-thread-calculator](https://vinkius.com/en/ai-agent-connect/embroidery-thread-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Embroidery Thread Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `embroidery-thread-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Embroidery Thread Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "embroidery-thread-calculator": {
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
