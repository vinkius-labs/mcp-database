# Ring Size Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ring-size-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Convert finger measurements into precise international ring sizes.

## Description
This MCP server provides high-precision ring sizing tools. Use `calculate_ring_size` to convert circumference or diameter into multiple international standards including US, UK, France, Germany, Japan, and Switzerland. It accounts for physiological factors like temperature-induced swelling and knuckle clearance, as well as stylistic needs like wide band adjustments.


## Available Tools (3)
- **calculate_ring_size**: Convert raw measurements into a comprehensive multi-system sizing report
- **convert_units**: Normalize different measurement types and units into a standard millimeter circumference and diameter
- **get_size_recommendation**: Provide a natural language summary and recommendation based on the calculated size and user constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ring Size Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my ring size if my finger circumference is 54mm and I want a US size?"

**🤖 AI Agent:**
> Your US ring size is 6.75.

---

**👤 You:**
> "Convert a 17mm diameter to UK size."

**🤖 AI Agent:**
> A 17mm diameter corresponds to a UK size N.

---

**👤 You:**
> "I have a 52mm circumference and a wide band of 8mm. What is my size?"

**🤖 AI Agent:**
> Your adjusted US ring size is 6.0.


## ❓ FAQ

**Q: How do I use the sizing tool?**
Provide your finger measurement (circumference or diameter) and the unit (mm or inches) to the `calculate_ring_size` tool to receive a full report.

**Q: Does it account for wide bands?**
Yes, if you specify a `bandWidth` greater than 6mm, the tool automatically adjusts the size for better comfort.

**Q: Can I adjust for temperature changes?**
Yes, you can enable `temperatureAdjustment` to account for fingers swelling in heat or shrinking in cold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ring-size-calculator](https://vinkius.com/ai-agent-connect/ring-size-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ring Size Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ring-size-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ring Size Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ring-size-calculator": {
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
