# Security Deposit Deductor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/security-deposit-deductor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate security deposit refunds by itemizing repair costs.

## Description
The Security Deposit Deductor MCP server allows landlords to accurately calculate the remaining balance of a security deposit after deducting verified repair costs. Using tools like `get_damage_summary`, you can see an itemized list of damages and whether total costs exceed the deposit. The `calculate_final_refund` tool determines the exact amount to return to tenants, ensuring all deductions are within the original deposit limit.


## Available Tools (3)
- **calculate_final_refund**: Determimines the exact monetary amount that should be returned to the tenant
- **get_damage_summary**: Provides a breakdown of all identified damages and identifies if the total costs exceed the available deposit
- **verify_damage_validity**: Validates that a single damage entry contains all necessary and actionable information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Security Deposit Deductor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a $1,000 deposit. There is a broken window for $200 and a wall scuff for $50. How much should I refund?"

**🤖 AI Agent:**
> The total damage cost is $250. Your final refund amount is $750.

---

**👤 You:**
> "Calculate the refund for a $500 deposit with damages: broken door ($300) and carpet stain ($300)."

**🤖 AI Agent:**
> The total damage cost is $600, which exceeds your $500 deposit. The amount to be deducted is $500, leaving a refund of $0.

---

**👤 You:**
> "Is a repair cost of -$50 for 'broken light' valid?"

**🤖 AI Agent:**
> No, the repair cost must be a non-negative number.


## ❓ FAQ

**Q: How does the tool calculate deductions?**
It sums all repair costs and subtracts them from the deposit, ensuring the deduction doesn't exceed the original amount.

**Q: Can I verify a single damage entry?**
Yes, use `verify_damage_validity` to check if a description and cost are valid.

**Q: What happens if damages exceed the deposit?**
The tool identifies that costs are over the deposit and calculates a refund of zero.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/security-deposit-deductor](https://vinkius.com/mcp/security-deposit-deductor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Security Deposit Deductor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `security-deposit-deductor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Security Deposit Deductor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "security-deposit-deductor": {
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
