# Project Fee Quote Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/project-fee-quote-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A precision tool for generating comprehensive project fee quotations by aggregating labor, materials, and margins.

## Description
This MCP server provides a suite of tools to build accurate project quotes. Use `calculate_labor_subtotal` to aggregate task costs, `calculate_material_subtotal` for direct expenses, and `apply_project_adjustments` to factor in revisions, contingency buffers, and target profit margins. Finally, use `calculate_final_quote` to generate the client-facing price including taxes.


## Available Tools (4)
- **calculate_final_quote**: Generates the final client-facing price including taxes
- **calculate_labor_subtotal**: Calculates the total cost of all planned labor tasks
- **calculate_material_subtotal**: Aggregates all direct material expenses
- **apply_project_adjustments**: Applies revisions, contingency, and target margin to the base costs to find the pre-tax amount


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Project Fee Quote Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the labor subtotal for 5 hours at $100/hr and 10 hours at $150/hr."

**🤖 AI Agent:**
> The labor subtotal is $2000.

---

**👤 You:**
> "I have a labor subtotal of $5000 and material costs of $1000. Apply a 1.1 revision multiplier, a 10% contingency, and a 20% target margin. What is the pre-tax total?"

**🤖 AI Agent:**
> The adjusted subtotal before tax is $7320.00.

---

**👤 You:**
> "What is the final price for a $5000 pre-tax amount with a 15% tax rate?"

**🤖 AI Agent:**
> The final price is $5750.00.


## ❓ FAQ

**Q: How does the tool handle profit margins?**
The tool uses a margin-based calculation via `apply_project_adjustments` to ensure the profit represents a specific percentage of the final price, rather than just adding a markup to the cost.

**Q: Can I include material costs in my quote?**
Yes, you can use `calculate_material_subtotal` to aggregate all direct material expenses before applying adjustments.

**Q: How are taxes applied?**
Taxes are applied to the pre-tax amount using the `calculate_final_quote` tool, which calculates the tax amount and the final grand total.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/project-fee-quote-builder](https://vinkius.com/en/ai-agent-connect/project-fee-quote-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Project Fee Quote Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `project-fee-quote-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Project Fee Quote Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "project-fee-quote-builder": {
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
