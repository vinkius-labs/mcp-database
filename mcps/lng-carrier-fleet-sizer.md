# LNG Carrier Fleet Sizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lng-carrier-fleet-sizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Optimize LNG fleet sizing and logistics planning.

## Description
This MCP server provides specialized tools for LNG logistics planning. It allows AI agents to determine optimal vessel fleets by calculating required vessel sizes and counts using `calculate_vessel_requirements`. Users can estimate operational cycles with `estimate_round_trip_time`, evaluate market risks via `analyze_charter_strategy`, and ensure terminal compatibility with `validate_regasification_sync`.


## Available Tools (4)
- **analyze_charter_strategy**: Compares the impact of using long-term versus spot charters on the delivery schedule
- **calculate_vessel_requirements**: Determines the necessary vessel size and the total number of vessels needed to fulfill the delivery goal
- **estimate_round_trip_time**: Calculates the duration of a single complete delivery cycle
- **validate_regasification_sync**: Checks if the vessel arrival frequency matches the regasification capacity at the destination


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LNG Carrier Fleet Sizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many vessels do I need for 5,000,000 m3 of LNG over 1 year with a 0.1% boil-off rate and 10,000 km distance?"

**🤖 AI Agent:**
> To deliver 5,000,000 m3 with those parameters, you will need a fleet of 4 vessels with a capacity of 140,000 m3 each.

---

**👤 You:**
> "What is the round trip time for a vessel traveling 5,000 km at 15 knots with 2 days of port stay?"

**🤖 AI Agent:**
> The total round-trip time is 12.4 days.

---

**👤 You:**
> "Should I use a long-term or spot charter if market volatility is high?"

**🤖 AI Agent:**
> With a high market volatility index, a long-term charter is recommended to ensure cost stability, even though it offers lower flexibility.


## ❓ FAQ

**Q: How do I calculate the number of vessels needed?**
You can use the `calculate_vessel_requirements` tool by providing the total volume, shipping distance, boil-off rate, and delivery schedule.

**Q: Can I check if my regasification plant can handle the arrivals?**
Yes, the `validate_regasification_sync` tool checks if vessel arrival frequency matches the regasification capacity.

**Q: Does this tool account for cargo loss during transit?**
Yes, the `calculate_vessel_requirements` tool incorporates the boil-off rate to ensure the delivered volume meets requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lng-carrier-fleet-sizer](https://vinkius.com/en/ai-agent-connect/lng-carrier-fleet-sizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LNG Carrier Fleet Sizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lng-carrier-fleet-sizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LNG Carrier Fleet Sizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lng-carrier-fleet-sizer": {
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
