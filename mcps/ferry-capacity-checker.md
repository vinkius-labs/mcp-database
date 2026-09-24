# Ferry Capacity Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ferry-capacity-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Monitor ferry occupancy and manage boarding requests in real-time.

## Description
This MCP server provides real-time maritime capacity management. It allows AI agents to monitor vessel occupancy, check available spaces, and validate boarding requests to ensure safety and operational efficiency. Use `get_vessel_capacity` to find limits, `check_remaining_space` to see available spots, and `validate_boarding_request` to confirm if a group can safely board.


## Available Tools (4)
- **check_remaining_space**: Calculates how many more passengers can board a specific ferry
- **get_fleet_utilization_status**: Provides a high-level overview of how many vessels in the fleet are near or at capacity
- **get_vessel_capacity**: Retrieves the maximum passenger capacity for a specific ferry
- **validate_boarding_request**: Determines if a group of passengers is allowed to board a ferry based on current status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ferry Capacity Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many more passengers can fit on ferry V-102 if there are currently 45 people on board?"

**🤖 AI Agent:**
> There are 55 spaces remaining on ferry V-102.

---

**👤 You:**
> "Can a group of 10 people board ferry V-500 if it already has 95 passengers and a capacity of 100?"

**🤖 AI Agent:**
> No, the group cannot board because the total occupancy would exceed the vessel's capacity.

---

**👤 You:**
> "What is the maximum capacity for vessel B-77?"

**🤖 AI Agent:**
> The maximum capacity for vessel B-77 is 200 passengers.


## ❓ FAQ

**Q: How can I check if a ferry is full?**
You can use the `check_remaining_space` tool to see how many spots are left or if the vessel is currently full.

**Q: Can I validate a group of passengers before they board?**
Yes, the `validate_boarding_request` tool determines if a specific number of passengers can safely board based on current occupancy.

**Q: How do I see the overall fleet status?**
Use `get_fleet_utilization_status` to get a high-level overview of how many vessels are near capacity or overloaded.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ferry-capacity-checker](https://vinkius.com/en/ai-agent-connect/ferry-capacity-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ferry Capacity Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ferry-capacity-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ferry Capacity Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ferry-capacity-checker": {
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
