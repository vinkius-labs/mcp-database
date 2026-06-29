# Incoterms 2020 Cost & Risk Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/incoterms-2020-cost-risk-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate logistics cost breakdowns, risk transfer points, and responsibility matrices for Incoterms 2020.

## Description
This MCP server provides a precise way to calculate the distribution of logistics costs, customs responsibilities, and risk transfer points based on Incoterms 2020. Use `calculate_cost_breakdown` to determine total expenses for both seller and buyer, including freight, insurance, and duties. Use `compare_risk_exposure` to analyze how risk shifts between different terms like FOB or DDP. Additionally, `get_responsibility_matrix` allows you to inspect exactly which party is responsible for tasks such as export clearance and loading.


## Available Tools (3)
- **calculate_cost_breakdown**: Calculate the total cost breakdown for a specific Incoterm
- **compare_risk_exposure**: g., comparing FOB vs DDP).

Compare risk transfer points between multiple Incoterms
- **get_responsibility_matrix**: Get the responsibility matrix for a specific Incoterm


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Incoterms 2020 Cost & Risk Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost breakdown for an FOB shipment with a goods value of 5000, freight of 500, and insurance of 100?"

**🤖 AI Agent:**
> For the FOB shipment, the total seller cost is $5,000 and the total buyer cost is $600 (freight and insurance).

---

**👤 You:**
> "Compare the risk transfer points for CIF and DDP."

**🤖 AI Agent:**
> For CIF, the risk transfers when the goods are on board the vessel. For DDP, the risk transfers at the named place of destination.

---

**👤 You:**
> "Who is responsible for export clearance under EXW?"

**🤖 AI Agent:**
> Under EXW, the buyer is responsible for handling all export clearance and documentation.


## ❓ FAQ

**Q: How does the cost breakdown calculation work?**
The `calculate_cost_breakdown` tool uses the selected Incoterm to allocate expenses like freight, insurance, and duties to either the seller or the buyer.

**Q: Can I compare multiple Incoterms at once?**
Yes, you can use the `compare_risk_exposure` tool by providing a list of Incoterm codes to see how risk transfer points differ.

**Q: Does the tool cover customs responsibilities?**
Yes, the `get_responsibility_matrix` tool provides a detailed breakdown of which party is responsible for tasks like export and import clearance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/incoterms-2020-cost-risk-calculator](https://vinkius.com/mcp/incoterms-2020-cost-risk-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Incoterms 2020 Cost & Risk Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `incoterms-2020-cost-risk-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Incoterms 2020 Cost & Risk Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "incoterms-2020-cost-risk-calculator": {
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
