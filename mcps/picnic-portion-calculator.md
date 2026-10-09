# Picnic Portion Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/picnic-portion-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate food portions and bulk serving units for events.

## Description
This MCP server provides tools to translate guest counts and per-person consumption estimates into actionable food quantities. Use `calculate_total_portions` to find the raw count, `convert_to_serving_units` to determine how many packs to buy, `validate_event_scale` to check capacity, or `get_portion_summary` for a complete overview of requirements.


## Available Tools (4)
- **calculate_total_portions**: Determines the raw total number of food portions needed for an event
- **convert_to_serving_units**: Converts individual portions into bulk serving units for easier procurement
- **get_portion_summary**: Provides a human-readable summary of the food requirements
- **validate_event_scale**: Checks if the requested portions are within a reasonable range for a single picnic event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Picnic Portion Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many portions do I need for 10 guests if each person eats 2 burgers?"

**🤖 AI Agent:**
> You need 20 portions in total.

---

**👤 You:**
> "If I need 20 portions and buns come in packs of 6, how many packs should I buy?"

**🤖 AI Agent:**
> You should buy 4 packs to ensure you have enough.

---

**👤 You:**
> "Give me a summary for 5 guests, 3 portions each, with 10 items per pack."

**🤖 AI Agent:**
> For 5 guests, you need 15 portions, which equals 2 packs of 10.


## ❓ FAQ

**Q: How do I calculate the total amount of food needed?**
You can use the `calculate_total_portions` tool by providing the guest count and the number of portions intended for each person.

**Q: Can I convert portions into bulk packs?**
Yes, the `convert_to_serving_units` tool converts individual portions into the number of bulk units or packs required based on the unit capacity.

**Q: Is there a way to get a full summary at once?**
Yes, use `get_portion_summary` to receive a human-readable summary including guest count, total portions, and total bulk units.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/picnic-portion-calculator](https://vinkius.com/en/ai-agent-connect/picnic-portion-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Picnic Portion Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `picnic-portion-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Picnic Portion Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "picnic-portion-calculator": {
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
