# Group Class Cost Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/group-class-cost-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equitably divide instructor, venue, material, tax, and payment fees among class participants.

## Description
This MCP server provides tools to calculate and distribute the total operational costs for group class sessions. It handles the aggregation of instructor fees, venue rentals, material costs, taxes, and payment processing fees to ensure every participant pays their fair share. Use `calculate_total_class_cost` to find the grand total, `split_cost_per_participant` to determine individual payments, `generate_cost_breakdown` for an itemized list, and `validate_participant_participation` to verify that collected funds cover all expenses.


## Available Tools (4)
- **calculate_total_class_cost**: Calculates the total sum of all expenses required to run the class
- **generate_cost_breakdown**: Provides a detailed itemized list of how the total cost was reached
- **split_cost_per_participant**: Determines exactly how much each individual needs to pay
- **validate_participant_participation**: Checks if a specific split configuration is mathematically sound and covers all costs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Group Class Cost Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for a class with a $500 instructor fee, $200 venue fee, $100 material fee, 10% tax, and a $15 payment fee?"

**🤖 AI Agent:**
> The total cost for the class is $855.00.

---

**👤 You:**
> "If the total cost is $450 and there are 10 participants, how much should each person pay?"

**🤖 AI Agent:**
> Each participant should pay $45.00.

---

**👤 You:**
> "Show me the breakdown for a class costing $1000 total, with $800 in core fees, $150 in tax, and $50 in processing fees."

**🤖 AI Agent:**
> The breakdown is: Subtotal: $800.00, Tax Amount: $150.00, Processing Fee: $50.00, Grand Total: $1000.00.


## ❓ FAQ

**Q: How does the tool handle taxes?**
The tax rate is applied to the subtotal of instructor, venue, and material fees before adding any flat payment processing fees.

**Q: Can I see a detailed list of all expenses?**
Yes, you can use the `generate_cost_breakdown` tool to receive an itemized list including the subtotal, tax amount, and processing fees.

**Q: How do I ensure I have collected enough money from participants?**
You can use `validate_participant_participation` to check if the sum of individual payments covers the total class cost.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/group-class-cost-splitter](https://vinkius.com/en/ai-agent-connect/group-class-cost-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Group Class Cost Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `group-class-cost-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Group Class Cost Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "group-class-cost-splitter": {
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
