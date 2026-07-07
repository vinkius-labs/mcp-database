# EV Range Anxiety Loop MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ev-range-anxiety-loop)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automotive](../categories/automotive.md)

Simulate EV battery depletion and calculate necessary charging stops.

## Description
This MCP server provides a simulation engine to predict battery depletion and calculate charging durations for electric vehicle trips. Using tools like `simulate_trip_drain`, `analyze_segment_safety`, and `calculate_recharge_duration`, you can model trip segments, evaluate the 20km safety buffer rule, and estimate time spent at various chargers based on their power output (kW). It is designed to help drivers plan routes that avoid range anxiety by identifying exactly where and for how long they need to stop.


## Available Tools (3)
- **calculate_recharge_duration**: Returns minutes required.

Calculate time needed to recharge
- **analyze_segment_safety**: Analyze if a trip segment triggers charging
- **simulate_trip_drain**: Returns total charging time and logs.

Simulate an entire EV trip with multiple charging stops


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EV Range Anxiety Loop** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will it take to recharge 50km if the charger is 50kW?"

**🤖 AI Agent:**
> It will take 60 minutes to recharge.

---

**👤 You:**
> "Will I need to charge if my current range is 100km and the next charger is 90km away?"

**🤖 AI Agent:**
> Yes, a charge event is triggered because the remaining range (100km) is less than the distance to the next charger (90km) plus the 20km buffer.

---

**👤 You:**
> "Simulate a trip starting with 200km range and chargers at 150km (50kW) and 250km (100kW)."

**🤖 AI Agent:**
> Total charging time: 60 minutes. Trip logs show a stop at 150km with 50km remaining range.


## ❓ FAQ

**Q: How does the safety buffer work?**
A charge event is triggered if the remaining range is insufficient to reach the next charger plus a 20km safety buffer.

**Q: Can I simulate multiple charging stops?**
Yes, by using the `simulate_trip_drain` tool with a JSON array of chargers along your route.

**Q: What inputs are required for charging duration?**
You need the range deficit in km and the charger speed in kW for `calculate_recharge_duration`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ev-range-anxiety-loop](https://vinkius.com/mcp/ev-range-anxiety-loop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EV Range Anxiety Loop** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ev-range-anxiety-loop` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EV Range Anxiety Loop** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ev-range-anxiety-loop": {
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
