# Rural Credit Simulator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rural-credit-simulator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Simulate agricultural credit scenarios, comparing programs like Pronaf and Pronamp with different amortization methods.

## Description
The Rural Credit Simulator is a specialized financial modeling tool designed to help producers and financial analysts evaluate the cost of agricultural financing. By using tools like `get_available_programs`, `simulate_repayment_plan`, and `compare_credit_options`, you can model complex credit scenarios involving different modalities such as Production Cost, Investment, and Marketing/Sales. The simulator accounts for various interest rate programs (including Pronaf and Pronamp), grace periods, and amortization systems like SAC, Price, and Bullet to provide a precise calculation of total costs and the Effective Total Cost (CET).


## Available Tools (3)
- **compare_credit_options**: Compare different credit programs for a single loan request
- **get_available_programs**: Retrieve a list of all supported agricultural credit programs
- **simulate_repayment_plan**: Simulate a loan repayment plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rural Credit Simulator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the available agricultural credit programs?"

**🤖 AI Agent:**
> The available programs are: Pronaf (low interest for small farmers), Pronamp (for medium producers), and Plano Safra.

---

**👤 You:**
> "Simulate a $50,000 loan for 24 months with a 6-month grace period using the Price method under Pronaf."

**🤖 AI Agent:**
> For a $50,000 loan under Pronaf for 24 months with a 6-month grace period using the Price method, the total cost will be approximately $58,450.20 with an effective annual cost of 12.5%.

---

**👤 You:**
> "Compare options for a $100,000 investment loan for 60 months."

**🤖 AI Agent:**
> Comparing the programs: Pronaf offers a total cost of $145,000, while Pronamp results in a total cost of $162,000 for this 60-month investment scenario.


## ❓ FAQ

**Q: How can I see which credit programs are available?**
You can use the `get_available_programs` tool to retrieve a complete list of supported programs, their interest rates, and the modalities they support.

**Q: Can I compare different financing options?**
Yes, the `compare_credit_options` tool allows you to input a loan amount and term to see a side-by-side comparison of total costs and effective rates across all available programs.

**Q: What amortization methods are supported?**
The simulator supports SAC (Systematic Amortization of Capital), Price (fixed installments), and Bullet (single lump sum payment) systems.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rural-credit-simulator](https://vinkius.com/mcp/rural-credit-simulator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rural Credit Simulator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rural-credit-simulator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rural Credit Simulator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rural-credit-simulator": {
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
