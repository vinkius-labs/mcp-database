# Stripping Ratio Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/stripping-ratio-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate critical stripping ratios and economic limits for open-pit mining operations.

## Description
This MCP server provides essential mining engineering calculations for open-pit operations. It allows AI agents to determine the long-term viability of a mine using `calculate_overall_stripping_ratio`, evaluate immediate costs via `calculate_incremental_stripping_ratio`, and identify economic limits with `calculate_break_even_stripping_ratio`. Additionally, it can estimate how pit wall geometry affects waste volumes through `analyze_slope_impact`.


## Available Tools (4)
- **analyze_slope_impact**: Estimates how changes in pit wall steepness affect the volume of waste required
- **calculate_break_even_stripping_ratio**: Identifies the economic limit for mining based on ore value and extraction costs
- **calculate_incremental_stripping_ratio**: Evaluates the immediate waste removal requirement for a specific mining stage or bench
- **calculate_overall_stripping_ratio**: Determines the total volume of waste relative to ore for the entire mine plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stripping Ratio Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the overall stripping ratio if I have 500,000 tons of waste and 100,000 tons of ore?"

**🤖 AI Agent:**
> The overall stripping ratio is 5.0.

---

**👤 You:**
> "Calculate the break-even stripping ratio if ore is worth $50 per ton and mining costs are $10 per ton."

**🤖 AI Agent:**
> The break-even stripping ratio is 4.0.

---

**👤 You:**
> "If I change my pit slope from 45 degrees to 50 degrees at a depth of 200 meters, how much will the waste volume change?"

**🤖 AI Agent:**
> The waste volume will decrease by approximately 12.5%.


## ❓ FAQ

**Q: What is the purpose of the Break-even Stripping Ratio?**
It identifies the maximum allowable stripping ratio before the cost of extracting ore exceeds its value, helping define the economic limit of the mine.

**Q: How does pit slope affect waste volume?**
Steeper pit slopes reduce the amount of waste that must be removed to reach the ore, whereas shallower slopes increase the waste volume.

**Q: Can I calculate the impact of changing my pit design?**
Yes, you can use the `analyze_slope_impact` tool to estimate the percentage change in waste volume when adjusting the pit wall angle.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/stripping-ratio-calculator](https://vinkius.com/ai-agent-connect/stripping-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stripping Ratio Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stripping-ratio-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stripping Ratio Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stripping-ratio-calculator": {
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
