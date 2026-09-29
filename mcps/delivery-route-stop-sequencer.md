# Delivery Route Stop Sequencer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/delivery-route-stop-sequencer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Optimize delivery routes by calculating efficient stop sequences and timing.

## Description
This MCP server provides an optimization engine to solve complex delivery routing problems. It uses a travel-time matrix, delivery windows, and service durations to determine the most efficient order of stops. You can use `calculate_optimal_sequence` to generate a full route timeline, `validate_route_constraints` to verify if a proposed route is feasible, `get_stop_efficiency_metrics` to analyze stop performance, and `estimate_route_window_buffer` to assess timing flexibility and risk levels.


## Available Tools (4)
- **calculate_optimal_sequence**: Determine the most efficient order of stops and calculate the full timeline of the route
- **estimate_route_window_buffer**: Determine how much flexibility exists in the current route before a stop becomes late
- **get_stop_efficiency_metrics**: Analyze the performance of a specific stop within a completed route
- **validate_route_constraints**: Check if a specific sequence of stops is physically possible given the time windows and service durations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Delivery Route Stop Sequencer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the best sequence for these stops: travel times [[0,10,20],[10,0,15],[20,15,0]], stops: [{'id':1,'windowStart':0,'windowEnd':30,'serviceTime':5},{'id':2,'windowStart':10,'windowEnd':40,'serviceTime':5}], depotIndex: 0, startTime: 0."

**🤖 AI Agent:**
> The optimal sequence is Stop 1 followed by Stop 2. Stop 1 arrives at 10, departs at 15. Stop 2 arrives at 30, departs at 35.

---

**👤 You:**
> "Is this route valid? Travel times [[0,5],[5,0]], stops: [{'id':1,'windowStart':0,'windowEnd':10,'serviceTime':5},{'id':2,'windowStart':2,'windowEnd':8,'serviceTime':5}], sequence: [0,1], startTime: 0."

**🤖 AI Agent:**
> The route is valid. Stop 1 is reached at 5 and Stop 2 is reached at 10.

---

**👤 You:**
> "What is the efficiency of a stop that arrived at 15 with a 5 minute travel time and 10 minute service duration?"

**🤖 AI Agent:**
> The stop has an idle ratio of 0.0 and a travel ratio of 0.33.


## ❓ FAQ

**Q: How do I find the best route for my drivers?**
You can use the `calculate_optimal_sequence` tool by providing the travel time matrix, stop requirements, and depot start time to get the most efficient sequence.

**Q: Can I check if a route is valid before sending it to a driver?**
Yes, the `validate_route_constraints` tool allows you to verify if a specific sequence of stops adheres to all delivery window and service duration constraints.

**Q: How can I see how much delay risk exists for a stop?**
Use the `estimate_route_window_buffer` tool to calculate the buffer time and risk level for any specific stop in your route.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/delivery-route-stop-sequencer](https://vinkius.com/en/ai-agent-connect/delivery-route-stop-sequencer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Delivery Route Stop Sequencer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `delivery-route-stop-sequencer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Delivery Route Stop Sequencer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "delivery-route-stop-sequencer": {
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
