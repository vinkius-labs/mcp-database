# Petrochemical Process Economics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/petrochemical-process-economics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Evaluate the financial viability and sensitivity of petrochemical production processes.

## Description
This MCP server provides a complete techno-economic modeling suite for petrochemical production. It allows AI agents to calculate total production costs using `get_production_cost`, determine profitability via `get_process_margin`, evaluate long-term investment viability with `calculate_project_npv`, and perform risk assessments through `run_sensitivity_analysis`. It accounts for CAPEX, OPEX, feedstock volatility, and scale effects to provide precise financial insights for chemical plant planning.


## Available Tools (4)
- **run_sensitivity_analysis**: Identifies which economic driver has the most significant impact on the project's NPV
- **calculate_project_npv**: Evaluates the long-term financial viability of the plant investment
- **get_process_margin**: Determines the profitability per unit of production
- **get_production_cost**: Calculates the total cost of producing a specific volume of product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Petrochemical Process Economics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total production cost for a plant with 500,000 unit capacity, $50 feedstock price, and $20 operating cost per unit?"

**🤖 AI Agent:**
> The total production cost for a capacity of 500,000 units is $35,000,000, with a unit cost of $70.

---

**👤 You:**
> "Calculate the margin if the unit cost is $70 and the product price is $100."

**🤖 AI Agent:**
> The margin per unit is $30, which represents a 30% margin percentage.

---

**👤 You:**
> "Evaluate a project with $10,000,000 investment, $2,000,000 annual cash flow, 10% discount rate, and 10 years life."

**🤖 AI Agent:**
> The Net Present Value (NPV) for this project is $2,355,000.


## ❓ FAQ

**Q: How does the tool handle scale effects?**
The `get_production_cost` tool incorporates scale effects by calculating the total production cost based on the provided capacity, ensuring that unit costs reflect the efficiencies of larger production volumes.

**Q: Can I perform risk assessment on my project?**
Yes, you can use `run_sensitivity_analysis` to identify which economic drivers, such as feedstock price or CAPEX, have the most significant impact on your project's NPV.

**Q: What inputs are needed for NPV calculation?**
To use `calculate_project_npv`, you must provide the initial investment (CAPEX), annual cash flow, the discount rate, and the total project life in years.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/petrochemical-process-economics](https://vinkius.com/en/ai-agent-connect/petrochemical-process-economics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Petrochemical Process Economics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `petrochemical-process-economics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Petrochemical Process Economics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "petrochemical-process-economics": {
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
