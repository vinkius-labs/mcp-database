# Square Footage Rent Comparer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/square-footage-rent-comparer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Fairly split monthly rent between roommates based on room square footage.

## Description
The Square Footage Rent Comparer is a precision-focused utility designed to help roommates divide monthly rent proportionally. By using the `compute_rent_distribution` tool, you can input your total rent and the square footage of each room to calculate an exact split that prevents rounding errors. You can also use `calculate_size_ratio` to see how much larger one room is than another, or `validate_split_parameters` to ensure your inputs are valid for a fair calculation.


## Available Tools (3)
- **calculate_size_ratio**: Answers how many times larger one room is compared to the other
- **compute_rent_distribution**: Determines the exact amount of rent each roommate should pay
- **validate_split_parameters**: Verifies that provided rent and area values are usable for a fair calculation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Square Footage Rent Comparer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If my total rent is $2,000 and Room A is 150 sqft while Room B is 250 sqft, how much should each person pay?"

**🤖 AI Agent:**
> Room A should pay $750.00 and Room B should pay $1,250.00.

---

**👤 You:**
> "How much larger is a 300 sqft room compared to a 150 sqft room?"

**🤖 AI Agent:**
> The 300 sqft room is 2 times larger than the 150 sqft room.

---

**👤 You:**
> "Check if my rent inputs are valid: $1500 total, Room A 100sqft, Room B -50sqft."

**🤖 AI Agent:**
> The input is invalid. The area for Room B must be a positive number.


## ❓ FAQ

**Q: How does the rent split calculation work?**
The tool calculates the total square footage of both rooms, determines Room A's proportion of that total, and multiplies it by the monthly rent. To ensure accuracy, Room B's portion is calculated as the remaining balance.

**Q: Can I use this for more than two rooms?**
Currently, this tool is specifically designed to compare and split rent between two specific rooms.

**Q: What happens if I enter zero or negative values?**
The `validate_split_parameters` tool will identify the error, as all inputs must be positive and non-zero for a valid calculation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/square-footage-rent-comparer](https://vinkius.com/mcp/square-footage-rent-comparer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Square Footage Rent Comparer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `square-footage-rent-comparer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Square Footage Rent Comparer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "square-footage-rent-comparer": {
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
