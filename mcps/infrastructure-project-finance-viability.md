# Infrastructure Project Finance Viability MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/infrastructure-project-finance-viability)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Calculate optimal capital structure and financial feasibility for large-scale infrastructure projects.

## Description
This MCP server provides specialized tools for infrastructure project finance modeling. It allows AI agents to determine the maximum debt capacity using `getMaxDebtCapacity`, calculate necessary equity via `calculateEquityRequirement`, and evaluate total profitability with `calculateProjectIrr`. The `validateFinanceViability` tool performs a holistic check to ensure projects meet both lender DSCR requirements and investor IRR targets, accounting for cash flow predictability and risk allocation.


## Available Tools (4)
- **calculateEquityRequirement**: Determines the necessary equity contribution required to fully fund the project
- **calculateProjectIrr**: Evaluates the total profitability of the project itself, independent of the capital structure
- **getMaxDebtCapacity**: Calculates the maximum amount of debt a project can carry based on cash flow and coverage constraints
- **validateFinanceViability**: Performs a holistic check to see if a project configuration meets all investor and lender constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infrastructure Project Finance Viability** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the maximum debt for a $100M project with $15M annual cash flow, a 1.5 DSCR requirement, and a predictability score of 0.9."

**🤖 AI Agent:**
> The maximum debt capacity for this project is $90,000,000, leaving a remaining equity gap of $10,000,000.

---

**👤 You:**
> "What is the equity needed for a $50M project if the max debt is $35M?"

**🤖 AI Agent:**
> The total equity required is $15,000,000, which represents 30% of the project cost.

---

**👤 You:**
> "Is a project with a $200M cost, $25M annual cash flows, and a target IRR of 12% viable if we use $150M debt?"

**🤖 AI Agent:**
> The project is viable as it meets the required IRR and maintains the necessary debt service coverage.


## ❓ FAQ

**Q: How does the tool handle cash flow volatility?**
The `getMaxDebtCapacity` tool uses a predictability score to adjust the maximum debt capacity, ensuring higher debt is only permitted for stable cash flows.

**Q: Can I validate a full project configuration?**
Yes, use `validateFinanceViability` to check if your proposed debt, equity, and cash flows satisfy both DSCR and IRR constraints.

**Q: What is the difference between Project IRR and Equity IRR in this model?**
The `calculateProjectIrr` tool evaluates the total profitability of the asset itself, independent of how it is financed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/infrastructure-project-finance-viability](https://vinkius.com/ai-agent-connect/infrastructure-project-finance-viability)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infrastructure Project Finance Viability** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infrastructure-project-finance-viability` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infrastructure Project Finance Viability** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infrastructure-project-finance-viability": {
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
