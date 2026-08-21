# Singapore Parking Fee Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/singapore-parking-fee-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate exact HDB and URA parking fees in Singapore.

## Description
This MCP server provides deterministic parking fee calculations for Singapore. It connects AI agents to local parking rate structures for HDB carparks and URA street parking. Use `calculate_parking_fee` to get the total cost, `get_rate_lookup_table` to check specific rates, or `validate_parking_session` to ensure a stay complies with local regulations.


## Available Tools (3)
- **calculate_parking_fee**: Calculates the total estimated parking fee for a specific stay
- **get_rate_lookup_table**: Retrieves the applicable rate per half-hour for a given configuration
- **validate_parking_session**: Validates if a parking session is valid according to local regulations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Singapore Parking Fee Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will it cost to park a Car in an HDB carpark from 2024-05-01T08:00:00Z to 2024-05-01T10:00:00Z on a weekday?"

**🤖 AI Agent:**
> The total fee for a Car in an HDB carpark for 2 hours is 2.40 SGD.

---

**👤 You:**
> "What is the rate for a Motorcycle in a URA street carpark during business hours?"

**🤖 AI Agent:**
> The applicable rate for a Motorcycle in a URA street carpark is 0.40 SGD per half hour.

---

**👤 You:**
> "Is my parking session valid for a Car in an HDB_season zone?"

**🤖 AI Agent:**
> Yes, the session is valid.


## ❓ FAQ

**Q: How do I calculate my total parking cost?**
You can use the `calculate_parking_fee` tool by providing the location type, vehicle type, and entry/exit timestamps.

**Q: Does this include weekend rates?**
Yes, the tool accounts for weekend and Public Holiday rates via the `isSaturdaySundayPH` parameter.

**Q: Can I check if my parking session is valid?**
Yes, use the `validate_parking_session` tool to check if your stay adheres to local regulations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/singapore-parking-fee-calculator](https://vinkius.com/ai-agent-connect/singapore-parking-fee-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Singapore Parking Fee Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `singapore-parking-fee-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Singapore Parking Fee Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "singapore-parking-fee-calculator": {
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
