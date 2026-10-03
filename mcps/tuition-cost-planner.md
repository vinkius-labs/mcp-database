# Tuition Cost Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tuition-cost-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total academic, living, and net costs with payment scheduling.

## Description
This MCP server provides a complete financial planning suite for students. It allows AI agents to calculate direct academic costs using `get_academic_costs`, estimate living expenses like housing and books via `get_living_and_material_costs`, and determine the final out-of-pocket amount with `calculate_net_obligation`. Additionally, it can generate a structured payment schedule using `get_payment_timeline` to help manage financial obligations throughout the term.


## Available Tools (4)
- **calculate_net_obligation**: Determines the final out-of-pocket amount after applying financial aid to all costs
- **get_living_and_material_costs**: Calculates the total cost of non-academic essentials like books, housing, and transport
- **get_academic_costs**: Calculates the total amount required for tuition and mandatory institutional fees
- **get_payment_timeline**: Maps out the specific dates when payments are due based on the student's term


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tuition Cost Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will my total academic cost be if I take 15 credits at $400 per credit and have $500 in mandatory fees?"

**🤖 AI Agent:**
> Your total academic cost will be $6,500.

---

**👤 You:**
> "Calculate my net cost if my total costs are $15,000 and I received $5,000 in scholarships."

**🤖 AI Agent:**
> Your net cost after applying the $5,000 scholarship is $10,000.

---

**👤 You:**
> "Create a payment schedule for $1,200 due on 2024-09-01 and 2024-12-01."

**🤖 AI Agent:**
> Your payment schedule is: $600 on 2024-09-01 and $600 on 2024-12-01.


## ❓ FAQ

**Q: How do I calculate my total tuition?**
You can use the `get_academic_costs` tool by providing your tuition rate per credit and the number of credits you are enrolled in.

**Q: Can I include my housing and book costs?**
Yes, the `get_living_and_material_costs` tool is designed to aggregate your expenses for books, housing, and transportation.

**Q: How does the tool handle financial aid?**
The `calculate_net_obligation` tool subtracts your total financial aid from your combined academic and living costs to find your final net cost.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tuition-cost-planner](https://vinkius.com/en/ai-agent-connect/tuition-cost-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tuition Cost Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tuition-cost-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tuition Cost Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tuition-cost-planner": {
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
