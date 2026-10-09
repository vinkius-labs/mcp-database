# Rent Increase Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/rent-increase-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate rent increases, stability, and multiple scenarios.

## Description
This MCP provides precise tools for managing rental adjustments. Use `calculate_rent_increase` to find the exact monetary increase and new total, `validate_rent_stability` to check if an increase is within market thresholds, `batch_calculate_scenarios` to compare multiple percentage steps, and `get_rent_percentage_difference` to find the change between two rent amounts.


## Available Tools (4)
- **batch_calculate_scenarios**: Generates a series of different rent outcomes for comparison purposes
- **calculate_rent_increase**: Calculates the specific monetary increase and the resulting new rent total
- **get_rent_percentage_difference**: Calculates the percentage difference between two different rent amounts
- **validate_rent_stability**: Determines if a proposed rent increase falls within common regulatory or market stability thresholds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rent Increase Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If my current rent is 1500 and it increases by 5%, what is the new rent?"

**🤖 AI Agent:**
> The increase amount is 75.00 and the new rent is 1575.00.

---

**👤 You:**
> "Is a 10% rent increase considered stable?"

**🤖 AI Agent:**
> No, a 10% increase is flagged as aggressive.

---

**👤 You:**
> "What is the percentage difference between a rent of 1000 and 1200?"

**🤖 AI Agent:**
> The percentage difference is 20%.


## ❓ FAQ

**Q: How do I calculate a specific rent increase?**
You can use the `calculate_rent_increase` tool by providing the current rent and the percentage you wish to apply.

**Q: Can I check if a rent increase is considered stable?**
Yes, the `validate_rent_stability` tool evaluates if an increase is negligible, moderate, or aggressive based on standard thresholds.

**Q: How can I compare multiple rent increase options at once?**
Use the `batch_calculate_scenarios` tool to pass a list of different percentage steps and see all resulting rent totals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/rent-increase-calculator](https://vinkius.com/en/ai-agent-connect/rent-increase-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rent Increase Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rent-increase-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rent Increase Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rent-increase-calculator": {
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
