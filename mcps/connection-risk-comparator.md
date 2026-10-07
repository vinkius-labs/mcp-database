# Connection Risk Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/connection-risk-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Assess flight connection reliability and buffer safety.

## Description
This MCP server provides tools to analyze flight connection risks. Use `evaluate_single_connection` to determine if a transfer meets the Minimum Connection Time (MCT), `compare_connection_options` to pick the safest itinerary, `calculate_buffer_fatigue` to see how delays impact your margin, and `get_airport_mct_lookup` to find required transfer times for specific airports.


## Available Tools (4)
- **calculate_buffer_fatigue**: Determines how much a delay in the first flight will erode the safety margin
- **compare_connection_options**: Compares two different connection itineraries to determine which offers better reliability
- **evaluate_single_connection**: Assesses the risk level of a single connection between two flights
- **get_airport_mct_lookup**: Provides the standard MCT for a specific airport and transfer scenario


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Connection Risk Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my connection at JFK safe if I land at 10:00 and depart at 11:30 with a terminal transfer and an MCT of 60 minutes?"

**🤖 AI Agent:**
> Yes, you have a 30-minute buffer after meeting the 60-minute MCT.

---

**👤 You:**
> "Compare two connections: Option A has a 45-minute buffer and Option B has a 20-minute buffer."

**🤖 AI Agent:**
> Option A is recommended as it provides a 25-minute larger buffer than Option B.

---

**👤 You:**
> "If I have a 30-minute buffer and my flight is delayed by 35 minutes, what is my status?"

**🤖 AI Agent:**
> Your status is Failed because the delay exceeds your available buffer.


## ❓ FAQ

**Q: How is connection risk calculated?**
Risk is calculated by comparing the time between arrival and departure against the airport's Minimum Connection Time (MCT).

**Q: Can I compare two different flight options?**
Yes, you can use `compare_connection_options` to see which itinerary provides a larger buffer and lower risk level.

**Q: What happens if a flight is delayed?**
You can use `calculate_buffer_fatigue` to determine if an expected delay will cause you to miss your connection.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/connection-risk-comparator](https://vinkius.com/en/ai-agent-connect/connection-risk-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Connection Risk Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `connection-risk-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Connection Risk Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "connection-risk-comparator": {
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
