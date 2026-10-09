# Laundry Load Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/laundry-load-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate washing machine cycles and load distributions based on clothing weight.

## Description
This MCP server provides tools to manage laundry planning. Use `get_load_distribution` to determine how many full cycles and partial loads are needed for a specific weight. You can also use `get_laundry_summary` for a natural language overview of your laundry requirements, or `validate_machine_suitability` to check if your machine capacity is being used efficiently. It also provides standard capacity tiers via `get_capacity_tiers` to help you select the right machine size.


## Available Tools (4)
- **get_capacity_tiers**: Provides standard machine capacity tiers for comparison
- **get_laundry_summary**: Provides a human-readable summary of the laundry requirements
- **get_load_distribution**: Calculates how many full cycles and what final partial weight are required
- **validate_machine_suitability**: Checks if a specific machine capacity is practical for a given total weight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Laundry Load Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 15kg of laundry and my machine capacity is 5kg. How many loads will I have?"

**🤖 AI Agent:**
> You will have 3 full loads.

---

**👤 You:**
> "My laundry weighs 7kg and my machine capacity is 10kg. Is this efficient?"

**🤖 AI Agent:**
> Yes, the load is efficient as it is at least eighty percent of the machine capacity.

---

**👤 You:**
> "Give me a summary for 12kg of laundry with a 5kg capacity machine."

**🤖 AI Agent:**
> You will need 2 full loads of 5kg and one final partial load of 2kg, for a total of 3 cycles.


## ❓ FAQ

**Q: How do I know if my machine is being used efficiently?**
You can use the `validate_machine_suitability` tool. It checks if the total weight is at least eighty percent of the machine's capacity.

**Q: Can I get a text summary of my laundry needs?**
Yes, the `get_laundry_summary` tool provides a human-readable summary including the number of full loads and the weight of any remaining partial load.

**Q: What information do I need to provide?**
Most tools require the total weight of the clothing and the maximum capacity of your washing machine.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/laundry-load-calculator](https://vinkius.com/en/ai-agent-connect/laundry-load-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Laundry Load Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `laundry-load-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Laundry Load Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "laundry-load-calculator": {
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
