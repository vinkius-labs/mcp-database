# Gaotie Seat Allocation Logic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/gaotie-seat-allocation-logic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Deterministic seat assignment calculator for Chinese High-Speed Rail (Gaotie).

## Description
This MCP server provides precise seat assignment logic for Chinese High-Speed Rail (Gaotie) services. It calculates optimal seat letters for passenger groups based on train class (G, D, or C) and service tier (Second, First, or Business). Use `calculate_seat_assignments` to find the best seat patterns for groups, `validate_seat_availability` to check if a specific seat letter exists in a class, or `get_layout_summary` to view the seating configuration. It ensures social cohesion by prioritizing adjacent seats for groups and window seats for individuals.


## Available Tools (3)
- **calculate_seat_assignments**: Determines the optimal seat letters for a specific group of passengers based on train and service class
- **get_layout_summary**: Provides a descriptive summary of the seating arrangement for a chosen class
- **validate_seat_availability**: Verifies if a specific seat letter is physically possible within a given service class


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gaotie Seat Allocation Logic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the best seats for 2 passengers in Second Class on a G train."

**🤖 AI Agent:**
> The optimal seats for your group are C and D.

---

**👤 You:**
> "Is seat B available in First Class?"

**🤖 AI Agent:**
> No, seat B is not available in First Class layouts.

---

**👤 You:**
> "What is the layout for Business Class?"

**🤖 AI Agent:**
> Business Class uses a specialized layout with available letters A, C, and F.


## ❓ FAQ

**Q: Which train classes are supported?**
The tool supports G (Gaotie), D (Dongche), and C (Chengche) train classes.

**Q: Can I check if a specific seat exists in First Class?**
Yes, you can use `validate_seat_availability` to verify if a seat letter like 'B' is valid for a specific service tier.

**Q: How does the tool handle groups of passengers?**
The `calculate_seat_assignments` tool prioritizes keeping passengers together by selecting adjacent seat letters to ensure social cohesion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/gaotie-seat-allocation-logic](https://vinkius.com/ai-agent-connect/gaotie-seat-allocation-logic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gaotie Seat Allocation Logic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gaotie-seat-allocation-logic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gaotie Seat Allocation Logic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gaotie-seat-allocation-logic": {
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
