# Group Tour Payment Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/group-tour-payment-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Schedules deposits and installment timelines for group travelers.

## Description
This MCP server provides financial scheduling tools for travel organizers. It allows AI agents to generate complete payment timelines using `get_payment_schedule`, calculate losses with `calculate_cancellation_penalty`, monitor group collection progress via `get_group_status`, and verify payment plans with `validate_installment_feasibility`.


## Available Tools (4)
- **get_payment_schedule**: Generates a complete timeline of all required payments for a single traveler
- **get_group_status**: Aggregates payment data for a whole group of travelers
- **validate_installment_feasibility**: Checks if a proposed set of installments is mathematically and logically sound
- **calculate_cancellation_penalty**: Determines how much money a traveler loses if they cancel on a specific date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Group Tour Payment Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a payment schedule for a $2000 tour with a $500 deposit and two installments of $750 on 2024-06-01 and 2024-08-01."

**🤖 AI Agent:**
> The payment schedule is: Deposit of $500, $750 due on 2024-06-01, and $750 due on 2024-08-01. Total cost is $2000.

---

**👤 You:**
> "What is the cancellation penalty for a traveler who paid $1000 and cancels on 2024-05-01 with a 20% penalty tier starting 2024-04-01?"

**🤖 AI Agent:**
> The non-refundable amount is $200, and the refundable amount is $800.

---

**👤 You:**
> "Show the status for a group of 5 travelers where each tour costs $1000 and John Doe has paid $500, Jane Smith has paid $1000, and others have paid $0."

**🤖 AI Agent:**
> The group has collected $1500 out of a total $5000. The collection progress is 30%.


## ❓ FAQ

**Q: How can I see the full payment timeline for a traveler?**
You can use the `get_payment_schedule` tool to generate a complete timeline including deposits and all future installments.

**Q: Can I check if my installment plan is valid?**
Yes, the `validate_installment_feasibility` tool checks if your proposed installments are mathematically and logically sound.

**Q: How do I calculate cancellation fees?**
Use the `calculate_cancellation_penalty` tool by providing the total amount paid and the specific cancellation date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/group-tour-payment-planner](https://vinkius.com/en/ai-agent-connect/group-tour-payment-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Group Tour Payment Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `group-tour-payment-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Group Tour Payment Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "group-tour-payment-planner": {
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
