# Metallurgical Accounting MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/metallurgical-accounting)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Precise metal balance, recovery reconciliation, and loss identification for mining operations.

## Description
This MCP server provides specialized tools for metallurgical accounting in mining and processing plants. It enables precise tracking of metal mass and grade through the entire circuit. Use `calculate_metal_balance` to determine the discrepancy between input and output, `reconcile_recovery` to compare actual performance against targets, `identify_losses` to isolate missing metal, and `validate_measurement_integrity` to ensure mass balances fall within acceptable error margins.


## Available Tools (4)
- **calculate_metal_balance**: Determines the total metal flow and identifies the discrepancy between input and output
- **identify_losses**: Specifically isolates and categorizes the missing metal within the system
- **reconcile_recovery**: Calculates the actual metallurgical recovery and compares it against a target performance level
- **validate_measurement_integrity**: Evaluates if the current mass balance is within acceptable bounds of measurement uncertainty


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Metallurgical Accounting** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the metal balance for a feed of 1000 tons at 2% grade, with a product of 200 tons at 10% grade and tails of 800 tons at 0.1% grade."

**🤖 AI Agent:**
> The feed metal is 20.0 units, the product metal is 20.0 units, and the tails metal is 0.8 units. The balance discrepancy is -0.8 units.

---

**👤 You:**
> "What is the recovery if I have 50 tons of product metal from 500 tons of feed metal, with a target of 85%?"

**🤖 AI Agent:**
> The actual recovery is 10.0%, which is Below Target compared to the 85.0% target.

---

**👤 You:**
> "Identify the losses if feed metal is 100, product metal is 85, and tails metal is 10."

**🤖 AI Agent:**
> The total loss is 5.0 units, and the identified losses are 5.0 units.


## ❓ FAQ

**Q: How do I calculate the metal balance?**
You can use the `calculate_metal_balance` tool by providing the feed tonnage, feed grade, a list of products (tonnage and grade), and the tails data.

**Q: Can I check if my measurement error is acceptable?**
Yes, the `validate_measurement_integrity` tool evaluates if the balance discrepancy is within your specified allowable error margin.

**Q: How are losses identified?**
The `identify_losses` tool isolates missing metal by comparing feed metal against the sum of product and tails metal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/metallurgical-accounting](https://vinkius.com/en/ai-agent-connect/metallurgical-accounting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Metallurgical Accounting** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `metallurgical-accounting` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Metallurgical Accounting** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "metallurgical-accounting": {
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
