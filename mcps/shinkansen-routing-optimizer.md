# Shinkansen Routing Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/shinkansen-routing-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Deterministic Japanese Shinkansen travel time and fare calculator.

## Description
This MCP server provides precise calculations for Shinkansen travel in Japan. Use `calculate_route_details` to find travel duration, intermediate stops, and transfer requirements. Use `calculate_fare_breakdown` to get a complete cost analysis including base fares, express surcharges, and Green Car upgrades. You can also use `check_jr_pass_eligibility` to verify if a specific train type is covered by a standard JR Pass.


## Available Tools (3)
- **calculate_fare_breakdown**: Determines the exact financial cost of the journey
- **calculate_route_details**: Calculates core travel metrics including time, stops, and transfer needs
- **check_jr_pass_eligibility**: Determines if the selected journey is covered by a standard JR Pass


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shinkansen Routing Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much does it cost to go from Tokyo to Kyoto on a Nozomi in Green Car?"

**🤖 AI Agent:**
> The total fare for a Green Car trip from Tokyo to Kyoto on the Nozomi is 22,500 JPY, consisting of a 14,000 JPY base fare, 6,500 JPY express surcharge, and 2,000 JPY Green Car upgrade fee.

---

**👤 You:**
> "How long is the trip from Shin-Osaka to Nagoya using the Kodama?"

**🤖 AI Agent:**
> The travel time from Shin-Osaka to Nagoya via Kodama is 50 minutes with 2 intermediate stops.

---

**👤 You:**
> "Is the Hikari train covered by a standard JR Pass?"

**🤖 AI Agent:**
> Yes, the Hikari train is fully covered by a standard JR Pass.


## ❓ FAQ

**Q: How do I calculate the total cost of my trip?**
You can use the `calculate_fare_breakdown` tool, which provides the base fare, express surcharge, and any Green Car upgrade fees to give you a total cost.

**Q: Is the Nozomi train covered by the JR Pass?**
You can verify this using `check_jr_pass_eligibility`. Generally, Nozomi requires a special supplement, while Hikari and Kodama are fully covered.

**Q: Can I see how many stops are between my stations?**
Yes, the `calculate_route_details` tool returns the exact number of intermediate stops between your origin and destination.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/shinkansen-routing-optimizer](https://vinkius.com/ai-agent-connect/shinkansen-routing-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shinkansen Routing Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shinkansen-routing-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shinkansen Routing Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shinkansen-routing-optimizer": {
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
