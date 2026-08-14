# Volume Profile Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/volume-profile-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic volume profile and market profile calculator.

## Description
This MCP server provides precise market structure analysis through volume-based calculations. It allows AI agents to generate detailed volume profiles, identify key liquidity levels, and analyze price action. Using `calculate_volume_profile`, agents can determine the Point of Control (POC), Value Area High (VAH), and Value Area Low (VAL). The `analyze_price_zones` tool identifies high volume nodes (HVN) and low volume nodes (LVN) to detect price acceptance or rejection. Additionally, `get_market_context` provides real-time positioning of price relative to the established value area.


## Available Tools (3)
- **analyze_price_zones**: Identifies areas where the market has either accepted or rejected price levels
- **calculate_volume_profile**: Generates the core volume distribution data and key market profile statistics
- **get_market_context**: Provides a summary of the current market structure relative to the volume profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Volume Profile Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the volume profile for these prices: [100, 101, 102, 100, 101] and volumes: [10, 20, 30, 10, 20] with 5 bins and a lookback of 5."

**🤖 AI Agent:**
> The Point of Control (POC) is at 102 with a volume of 30. The Value Area High (VAH) is 102 and the Value Area Low (VAL) is 100.

---

**👤 You:**
> "Analyze the price zones for this profile: {"poc": 150, "vah": 155, "val": 145, "hvn": [150], "lvn": [140]} with a sensitivity of 0.5."

**🤖 AI Agent:**
> The analysis shows an acceptance zone around the POC at 150 and a rejection zone at 140.

---

**👤 You:**
> "Is the current price of 152 inside the value area for a profile with VAH 155 and VAL 145?"

**🤖 AI Agent:**
> Yes, the current price of 152 is inside the Value Area.


## ❓ FAQ

**Q: What can I calculate with this tool?**
You can calculate the Point of Control (POC), Value Area (VAH/VAL), High Volume Nodes (HVN), Low Volume Nodes (LVN), and Initial Balance using the `calculate_volume_profile` tool.

**Q: How do I identify price rejection zones?**
Use the `analyze_price_zones` tool. It identifies rejection zones by looking for Low Volume Nodes (LVN) where price moves rapidly through areas of low liquidity.

**Q: Can I check if the current price is within the value area?**
Yes, the `get_market_context` tool provides a boolean indicating if the current price is inside the Value Area and describes its position relative to the POC.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/volume-profile-calculator](https://vinkius.com/mcp/volume-profile-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Volume Profile Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `volume-profile-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Volume Profile Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "volume-profile-calculator": {
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
