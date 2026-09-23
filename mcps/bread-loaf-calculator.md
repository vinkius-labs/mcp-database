# Bread Loaf Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bread-loaf-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [math](../categories/math.md)

Calculate production capacity, yield with wastage, and batch feasibility for bakery operations.

## Description
This MCP server provides essential tools for bakery production planning. It allows bakers to calculate how many full loaves can be produced from a specific dough weight using `get_production_capacity`. It also accounts for real-world dough loss with `calculate_yield_with_wastage`, checks if a specific production goal is achievable via `check_batch_feasibility`, and provides production planning scenarios through `get_production_tiers`.


## Available Tools (4)
- **calculate_yield_with_wastage**: Estimates the number of loaves possible after accounting for expected dough loss
- **check_batch_feasibility**: Determines if a specific production goal (number of loaves) is possible with the current dough supply
- **get_production_capacity**: Calculates how many full loaves can be produced from a given amount of dough
- **get_production_tiers**: Provides a breakdown of production potential at different wastage levels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bread Loaf Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many 500g loaves can I make from 10kg of dough?"

**🤖 AI Agent:**
> You can make 20 full loaves, with 0g of dough remaining.

---

**👤 You:**
> "If I have 5000g of dough and expect 5% wastage, how many 400g loaves can I produce?"

**🤖 AI Agent:**
> After 5% wastage, you will have 4750g of usable dough, allowing for 11 full loaves.

---

**👤 You:**
> "Do I have enough dough for 50 loaves of 800g each if I have 45kg of dough?"

**🤖 AI Agent:**
> Yes, you have enough dough. You will have a surplus of 5000g.


## ❓ FAQ

**Q: How does the tool handle dough wastage?**
The `calculate_yield_with_wastage` tool subtracts a specified percentage from the total dough weight before calculating the number of loaves, simulating real-world loss.

**Q: Can I check if I have enough dough for a specific order?**
Yes, use `check_batch_feasibility` to determine if your current dough supply can meet your required number of loaves.

**Q: What happens to the leftover dough?**
The `get_production_capacity` tool returns both the total number of full loaves and the `remainingDough` mass that was insufficient for a full loaf.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bread-loaf-calculator](https://vinkius.com/en/ai-agent-connect/bread-loaf-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bread Loaf Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bread-loaf-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bread Loaf Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bread-loaf-calculator": {
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
