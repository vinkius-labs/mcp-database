# Trip Emission Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/trip-emission-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Aggregate and analyze CO2e emissions from individual journey segments.

## Description
This MCP server provides tools to calculate the total carbon footprint of a journey by aggregating emissions from multiple legs. Use `calculate_trip_total` to sum up all segments, `get_emission_summary_by_type` to see the impact of specific transport modes like flights or trains, and `filter_high_emission_legs` to identify the most polluting parts of a trip. It is designed to help users understand the environmental impact of their travel through precise CO2e summation.


## Available Tools (4)
- **calculate_trip_total**: Calculate the total carbon footprint for the entire journey
- **filter_high_emission_legs**: Filter legs that exceed a specific emission threshold
- **get_emission_summary_by_type**: Get the total emissions and percentage contribution for a specific transport mode
- **validate_leg_format**: Validate if a specific journey segment is formatted correctly


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trip Emission Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total carbon footprint for this journey: a flight with 150 CO2e and a train ride with 20 CO2e?"

**🤖 AI Agent:**
> The total carbon footprint for this journey is 170 CO2e.

---

**👤 You:**
> "How much of my trip impact comes from flights if I have a flight with 200 CO2e and a car trip with 50 CO2e?"

**🤖 AI Agent:**
> The flight contribution is 200 CO2e, which represents 80% of the total trip impact.

---

**👤 You:**
> "Which legs of my trip had emissions higher than 40?"

**🤖 AI Agent:**
> The high emission legs are: Flight A (50 CO2e).


## ❓ FAQ

**Q: How do I calculate the total emissions for my trip?**
You can use the `calculate_trip_total` tool by providing an array of journey legs, where each leg contains its specific `emissionValue`.

**Q: Can I see which transport mode caused the most pollution?**
Yes, the `get_emission_summary_by_type` tool allows you to filter emissions by a specific mode, such as 'flight' or 'train', and see its contribution percentage.

**Q: How can I identify the most damaging parts of my journey?**
Use the `filter_high_emission_legs` tool with a chosen threshold to extract only the segments that exceed your specified emission limit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/trip-emission-total](https://vinkius.com/en/ai-agent-connect/trip-emission-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Trip Emission Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `trip-emission-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Trip Emission Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trip-emission-total": {
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
