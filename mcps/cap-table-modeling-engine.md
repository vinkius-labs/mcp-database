# Cap Table Modeling Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cap-table-modeling-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Precision modeling for equity ownership, dilution, and exit payouts.

## Description
This MCP server provides a precision modeling engine for simulating equity ownership, dilution, and exit payouts. It allows AI agents to model cap table evolution by simulating the conversion of convertible notes and SAFEs, calculating the impact of option pool expansions via `simulate_dilution`, and determining cash distributions through `calculate_exit_waterfall`. Use `query_current_ownership` to inspect the current state of the capitalization table.


## Available Tools (4)
- **calculate_exit_waterfall**: Determines the cash distribution to all shareholders during a liquidity event
- **convert_instruments**: Simulates the conversion of convertible notes and SAFEs into equity based on a target valuation and specific terms
- **query_current_ownership**: Retrieves the current ownership distribution of the company
- **simulate_dilution**: Models the impact of expanding the option pool or issuing new equity on existing ownership


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cap Table Modeling Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current ownership of the company?"

**🤖 AI Agent:**
> The current shareholders are: Alice (40%), Bob (30%), and the Employee Pool (30%).

---

**👤 You:**
> "How much will the shareholders receive if the company is sold for $50,000,000?"

**🤖 AI Agent:**
> Based on the exit waterfall, Alice will receive $20,000,000, Bob will receive $15,000,000, and the Employee Pool will receive $15,000,000.

---

**👤 You:**
> "What happens to ownership if we increase the option pool to 15%?"

**🤖 AI Agent:**
> Increasing the option pool to 15% will result in Alice's ownership moving from 40% to 34%, Bob's from 30% to 25.5%, and the Employee Pool from 30% to 25.5%.


## ❓ FAQ

**Q: How can I see the current ownership distribution?**
You can use the `query_current_ownership` tool to retrieve a detailed list of shareholders, their shares owned, and their current ownership percentages.

**Q: How does the tool handle convertible note conversion?**
The `convert_instruments` tool calculates the conversion price by selecting the lower of the price derived from the valuation cap or the price derived from the discount rate.

**Q: Can I simulate the impact of a new funding round?**
Yes, use `simulate_dilution` to model how expanding the option pool or issuing new equity affects existing ownership percentages.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cap-table-modeling-engine](https://vinkius.com/en/ai-agent-connect/cap-table-modeling-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cap Table Modeling Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cap-table-modeling-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cap Table Modeling Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cap-table-modeling-engine": {
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
