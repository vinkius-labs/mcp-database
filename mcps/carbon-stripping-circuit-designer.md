# Carbon Stripping Circuit Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/carbon-stripping-circuit-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design gold elution circuits by calculating vessel sizes, timing, and reagent needs.

## Description
This MCP server provides specialized engineering tools for designing gold recovery elution circuits. It allows users to calculate critical parameters for both Zadra and AARL stripping methods. Use `strip_vessel_sizing` to determine physical vessel dimensions, `elution_timing` to predict cycle durations based on temperature and pressure, and `reagent_consumption_calc` to estimate chemical requirements. The suite also includes `circuit_efficiency_check` to validate design performance against gold loading and operating conditions.


## Available Tools (1)
- **strip_vessel_sizing**: Calculates the required physical size of the stripping vessel or columns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Carbon Stripping Circuit Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the vessel size for a Zadra process with a throughput of 50 m3/h."

**🤖 AI Agent:**
> The required vessel for the Zadra process at 50 m3/h is 120 m3 with a diameter of 4.5m and a height of 7.5m.

---

**👤 You:**
> "How long will the elution take for an AARL process with 10 units of gold capacity at 95 degrees Celsius?"

**🤖 AI Agent:**
> The total elution duration is 480 minutes with 2 required cycles.

---

**👤 You:**
> "Estimate reagent needs for a Zadra circuit with 20 m3 of carbon."

**🤖 AI Agent:**
> The estimated total reagent volume is 150 m3 with a flow rate of 15 m3/h.


## ❓ FAQ

**Q: What stripping methods are supported?**
The server supports both the Zadra batch process and the AARL continuous elution process.

**Q: How do I calculate the required vessel size?**
You can use the `strip_vessel_sizing` tool by providing the stripping method and the circuit throughput.

**Q: Can I account for temperature in my timing calculations?**
Yes, the `elution_timing` tool uses operating temperature and pressure to determine the total duration of the stripping cycle.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/carbon-stripping-circuit-designer](https://vinkius.com/ai-agent-connect/carbon-stripping-circuit-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Carbon Stripping Circuit Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `carbon-stripping-circuit-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Carbon Stripping Circuit Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "carbon-stripping-circuit-designer": {
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
