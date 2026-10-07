# City Pass Value Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/city-pass-value-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare city tourist passes against individual attraction and transport costs.

## Description
This MCP server provides analytical tools to determine if a city tourist pass is financially beneficial for your planned itinerary. Use `analyze_itinerary_value` to compare the total cost of individual tickets against the best available pass. You can also use `check_pass_coverage` to verify if specific activities are included in a pass, `calculate_itinerary_duration` to find the time span of your trip, and `get_break_even_analysis` to see how many more attractions you need to visit to make a pass worth the investment.


## Available Tools (4)
- **analyze_itinerary_value**: Calculates the total cost of individual tickets versus the best available city pass for a specific itinerary
- **check_pass_coverage**: Verifies if a specific city pass covers a specific planned activity
- **calculate_itinerary_duration**: Determines the total span of time required to complete an itinerary
- **get_break_even_analysis**: Identifies how many more attractions of a certain type are needed to make a pass financially viable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **City Pass Value Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Should I buy a 48-hour city pass for my trip to London?"

**🤖 AI Agent:**
> Based on your planned activities, the 48-hour city pass will save you $25 compared to buying individual tickets for the British Museum, London Eye, and your metro trips.

---

**👤 You:**
> "How many more museums do I need to visit to make the museum pass worth it?"

**🤖 AI Agent:**
> You need to visit 2 more museums at an average cost of $15 each to reach the break-even point for the museum pass.

---

**👤 You:**
> "Does the standard city pass cover my bus trips?"

**🤖 AI Agent:**
> Yes, the standard city pass includes coverage for all local bus and metro transport.


## ❓ FAQ

**Q: How does the tool determine if a pass is worth it?**
The tool calculates the sum of all individual attraction and transport costs in your itinerary and compares it to the price of compatible city passes. A pass is considered 'worth it' if its price is lower than the individual costs of the activities it covers.

**Q: What makes a pass 'compatible' with my itinerary?**
A pass is compatible if the time elapsed between your first and last planned activity does not exceed the pass's validity period, and if the pass covers the categories of the activities you have planned.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, this MCP server can be connected to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/city-pass-value-comparator](https://vinkius.com/en/ai-agent-connect/city-pass-value-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **City Pass Value Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `city-pass-value-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **City Pass Value Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "city-pass-value-comparator": {
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
