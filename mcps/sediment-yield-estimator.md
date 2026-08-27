# Sediment Yield Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sediment-yield-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental-science](../categories/environmental-science.md)

Estimates sediment yield from erosion and delivery using USLE and MUSLE models.

## Description
This MCP server provides specialized tools for hydrological and geological modeling. It allows AI agents to calculate annual sediment yield using `calculate_annual_yield`, estimate event-based sediment production with `calculate_event_yield`, and determine sediment concentration in runoff. It also includes tools to calculate the `calculate_trapping_requirement` for sediment control structures and to `evaluate_erosion_sources` by distinguishing between upslope and channel erosion contributions.


## Available Tools (5)
- **calculate_annual_yield**: Calculate the expected annual sediment yield for a catchment
- **calculate_event_yield**: Calculate the sediment yield produced during a specific storm or erosion event
- **calculate_sediment_concentration**: Calculate the density of sediment within the runoff water
- **calculate_trapping_requirement**: Calculate the required sediment capture to meet a specific target
- **evaluate_erosion_sources**: Evaluate the contribution of upslope erosion versus channel erosion


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sediment Yield Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected annual sediment yield for a catchment with 5 tonnes/ha soil loss, a 0.2 delivery ratio, and a 500 hectare area?"

**🤖 AI Agent:**
> The expected annual sediment yield is 500 tonnes per year.

---

**👤 You:**
> "How much sediment will be produced in a storm event with 10 tonnes of MUSLE soil loss, a 0.15 delivery ratio, and a 100 hectare drainage area?"

**🤖 AI Agent:**
> The event sediment yield is 15 tonnes.

---

**👤 You:**
> "If I have 100 tonnes of sediment yield and want to reduce it to 20 tonnes, what trapping efficiency do I need?"

**🤖 AI Agent:**
> A trapping efficiency of 0.8 (or 80%) is required to meet the target.


## ❓ FAQ

**Q: What is the difference between the annual and event-based tools?**
The `calculate_annual_yield` tool uses USLE for long-term average annual erosion, while `calculate_event_yield` uses MUSLE for specific storm or erosion events.

**Q: How can I determine if a dam is sufficient for my target?**
You can use `calculate_trapping_requirement` to find the exact fraction of sediment that must be intercepted to reach your desired target yield.

**Q: Can I analyze where sediment is coming from?**
Yes, the `evaluate_erosion_sources` tool allows you to determine the ratio between upslope erosion and channel erosion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sediment-yield-estimator](https://vinkius.com/ai-agent-connect/sediment-yield-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sediment Yield Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sediment-yield-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sediment Yield Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sediment-yield-estimator": {
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
