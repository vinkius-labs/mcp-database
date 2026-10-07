# Weekend Getaway Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/weekend-getaway-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Rank and compare short-trip destinations based on travel time, cost, and personal preferences.

## Description
This MCP server provides decision-support tools to help you plan the perfect short trip. You can use `get_destination_options` to see available locations, `calculate_trip_rankings` to find the best matches based on your specific weights for time, cost, and weather, or `compare_two_destinations` to see a side-by-side metric comparison between two specific spots.


## Available Tools (4)
- **compare_two_destinations**: Provides a side-by-side comparison of two specific destinations
- **calculate_trip_rankings**: Calculates a ranked list of destinations based on specific user preferences and weights
- **get_destination_details**: Provides a deep dive into a specific destination's metrics
- **get_destination_options**: Retrieves a list of available getaway destinations and their specific attributes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weekend Getaway Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are some good getaway options in the North region?"

**🤖 AI Agent:**
> The available destinations in the North region are Alpine Retreat and Lakeside Cabin.

---

**👤 You:**
> "Rank destinations for me. I want sunny weather and I care most about low cost."

**🤖 AI Agent:**
> Based on your preference for sunny weather and low cost, the top ranked destination is Sunny Valley.

---

**👤 You:**
> "Compare destination ID 'city-a' and 'city-b'."

**🤖 AI Agent:**
> City A has a travel time 2 hours shorter than City B, but City B offers 3 hours more activity time.


## ❓ FAQ

**Q: How do I rank destinations?**
You can use the `calculate_trip_rankings` tool by providing your preferred weather and importance weights for factors like cost and travel time.

**Q: Can I filter destinations by region?**
Yes, use `get_destination_options` and provide a region name to filter the available getaway locations.

**Q: How do I compare two specific places?**
Use the `compare_two_destinations` tool with the unique IDs of the two destinations you want to evaluate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/weekend-getaway-comparator](https://vinkius.com/en/ai-agent-connect/weekend-getaway-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weekend Getaway Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weekend-getaway-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weekend Getaway Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weekend-getaway-comparator": {
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
