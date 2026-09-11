# LNG Project Economics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lng-project-economics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Economic analysis for LNG value chains, including delivered cost, NPV, and break-even price.

## Description
This MCP server provides specialized economic modeling for the Liquefied Natural Gas (LNG) industry. It connects AI agents to an integrated chain model that evaluates the entire value chain from gas supply to regasification. Use `calculate_delivered_cost` to determine landed prices, `calculate_project_npv` to assess lifetime profitability, `calculate_break_even_price` to find the minimum viable market price, and `analyze_chain_efficiency` to pinpoint the most expensive segment of the LNG chain.


## Available Tools (4)
- **analyze_chain_efficiency**: Compares the cost contributions of different stages in the LNG chain
- **calculate_break_even_price**: Identifies the minimum market price required to make the project economically viable
- **calculate_delivered_cost**: Determines the total cost to deliver one unit of LNG to the destination terminal
- **calculate_project_npv**: Evaluates the total lifetime profitability of the LNG project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LNG Project Economics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the delivered cost per unit if gas supply is 2.0, CAPEX is 500, OPEX is 50, capacity is 5, shipping is 10 per trip with 10 trips per year, and regasification is 1.5?"

**🤖 AI Agent:**
> The total delivered cost per unit is 15.5.

---

**👤 You:**
> "Calculate the NPV for a project with 100 annual revenue, 60 annual operating cost, 200 initial investment, 10 years life, and 5% discount rate."

**🤖 AI Agent:**
> The Net Present Value (NPV) for this project is 151.58.

---

**👤 You:**
> "Which part of the LNG chain is most expensive if gas cost is 3, liquefaction OPEX is 2, shipping is 5, and regasification is 1, with an annual capacity of 10?"

**🤖 AI Agent:**
> The most expensive segment is shipping.


## ❓ FAQ

**Q: What can this MCP server calculate?**
It calculates delivered LNG costs, project Net Present Value (NPV), break-even gas prices, and identifies the most expensive segments in the LNG value chain using `analyze_chain_efficiency`.

**Q: How does it handle shipping costs?**
The `calculate_delivered_cost` tool incorporates shipping costs by taking the cost per trip and the number of trips per year into account.

**Q: Is this suitable for large-scale project modeling?**
Yes, the model accounts for annual capacity and capital expenditures, making it suitable for modeling both small-scale and large-scale LNG projects.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lng-project-economics](https://vinkius.com/en/ai-agent-connect/lng-project-economics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LNG Project Economics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lng-project-economics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LNG Project Economics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lng-project-economics": {
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
