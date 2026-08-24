# Airline Baggage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/airline-baggage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Calculate baggage allowances and excess fees based on airline, fare class, and route.

## Description
This MCP server provides a deterministic engine to determine passenger baggage entitlements. Use `calculate_baggage_allowance` to find checked bag counts and weight limits, `estimate_excess_fees` to calculate penalties for overweight or oversize luggage, and `get_carry_on_rules` to check cabin constraints. It accounts for airline policies, fare classes, route types, and loyalty status.


## Available Tools (3)
- **calculate_baggage_allowance**: Determine the total permitted baggage for a passenger
- **estimate_excess_fees**: Calculate the cost of overweight or oversize luggage
- **get_carry_on_rules**: Retrieve specific cabin baggage constraints for a passenger


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Airline Baggage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my baggage allowance for a United Airlines economy flight from New York to London?"

**🤖 AI Agent:**
> For a United Airlines (UA) economy flight on a transatlantic route, you are allowed 1 checked bag with a 23kg weight limit.

---

**👤 You:**
> "How much will it cost if my bag is 28kg on an American Airlines flight?"

**🤖 AI Agent:**
> The overweight fee for a 28kg bag on American Airlines (AA) is $50.00.

---

**👤 You:**
> "What are the carry-on rules for Lufthansa business class?"

**🤖 AI Agent:**
> For Lufthansa (LH) business class, you are allowed one carry-on bag with a maximum weight of 8kg and a linear dimension limit of 115cm.


## ❓ FAQ

**Q: How do I check my checked bag allowance?**
You can use the `calculate_baggage_allowance` tool by providing your airline code, fare class, and route type.

**Q: Does loyalty status affect my baggage?**
Yes, if you have Silver, Gold, or Platinum status, the `calculate_baggage_allowance` tool will increase your checked bag count by one.

**Q: How can I estimate fees for an overweight bag?**
Use the `estimate_excess_fees` tool with the bag's actual weight and the airline's weight limit to get a precise USD estimate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/airline-baggage-calculator](https://vinkius.com/ai-agent-connect/airline-baggage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Airline Baggage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `airline-baggage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Airline Baggage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "airline-baggage-calculator": {
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
