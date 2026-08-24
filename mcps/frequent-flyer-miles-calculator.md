# Frequent Flyer Miles Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/frequent-flyer-miles-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise airline mileage accrual, including base miles, bonus miles, and EQM.

## Description
This MCP server provides deterministic tools for calculating frequent flyer mileage accrual. It bridges AI agents to airline loyalty logic, allowing for precise calculations of base miles, bonus miles based on fare class multipliers, and Elite Qualification Miles (EQM). Use `calculate_flight_distance` to find the distance between IATA codes, `get_program_rules` to fetch airline-specific multipliers, and `calculate_mileage_accrual` to get the final breakdown of redeemable and status-qualifying miles.


## Available Tools (3)
- **calculate_flight_distance**: Determines the physical distance of a flight between two IATA airport codes
- **calculate_mileage_accrual**: Calculates the specific breakdown of miles earned for a single flight segment
- **get_program_rules**: Retrieves the specific multipliers and constants for a given airline program


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Frequent Flyer Miles Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many miles will I earn for a 1200 mile flight with a Y fare class on AAdvantage?"

**🤖 AI Agent:**
> You will earn 2,400 total redeemable miles (1,200 base miles and 1,200 bonus miles) and 1,200 EQM.

---

**👤 You:**
> "What is the distance between JFK and LAX?"

**🤖 AI Agent:**
> The great-circle distance between JFK and LAX is approximately 2,475 miles.

---

**👤 You:**
> "Calculate accrual for a 300 mile domestic flight with fare class Q on SkyMiles."

**🤖 AI Agent:**
> You will earn 500 total redeemable miles (due to the domestic minimum guarantee) and 300 EQM.


## ❓ FAQ

**Q: How are bonus miles calculated?**
Bonus miles are calculated by applying a specific multiplier to the base miles, which is determined by the airline program and the fare class used for booking.

**Q: Does this tool handle domestic flight guarantees?**
Yes, the `calculate_mileage_accrual` tool applies a minimum mile guarantee of 500 miles for domestic flights to ensure a baseline accrual.

**Q: What is the difference between redeemable miles and EQM?**
Redeemable miles are the total miles you can spend on rewards, including bonuses. EQM (Elite Qualification Miles) are the miles used to determine your tier status within a loyalty program.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/frequent-flyer-miles-calculator](https://vinkius.com/ai-agent-connect/frequent-flyer-miles-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Frequent Flyer Miles Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `frequent-flyer-miles-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Frequent Flyer Miles Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "frequent-flyer-miles-calculator": {
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
