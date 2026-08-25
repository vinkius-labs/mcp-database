# Accelerator Follow-on Fund Modeler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-follow-on-fund-modeler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Project fund economics, deployment capacity, and return scenarios for accelerator follow-on funds.

## Description
This MCP server provides specialized financial modeling for accelerator funds. It allows AI agents to calculate deployable capital, manage pro-rata reserves, and simulate various exit scenarios. Use `calculate_deployment_capacity` to determine investable capital after fees and reserves, `project_return_scenarios` to estimate investor returns and manager carry, and `model_recycling_impact` to see how reinvesting exit proceeds increases total deployment capacity.


## Available Tools (3)
- **project_return_scenarios**: Estimates the potential returns to investors and carry to managers based on different success outcomes
- **calculate_deployment_capacity**: Determines how much capital is available for investment and how much must be reserved for follow-on rights
- **model_recycling_impact**: Calculates how reinvesting realized gains affects the total capital available for deployment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Follow-on Fund Modeler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the deployment capacity for a $50M fund with a 2% management fee, 20 companies, and $1M follow-on allocation per company."

**🤖 AI Agent:**
> The deployable capital is $40,000,000, with total pro-rata reserves of $20,000,000 and net investable capital of $20,000,000.

---

**👤 You:**
> "What are the returns for $10M invested if we have exit multiples of 0.0, 3.0, and 10.0 with a 20% carry rate?"

**🤖 AI Agent:**
> At a 0.0x multiple, the fund value is $0. At a 3.0x multiple, the fund value is $30,000,000. At a 10.0x multiple, the fund value is $100,000,000.

---

**👤 You:**
> "Show the impact of recycling for a fund with $10M deployable capital, a 50% exit rate, and an average 3x exit multiple."

**🤖 AI Agent:**
> The total capital deployed with recycling is $15,000,000, resulting in an incremental capital gain of $5,000,000.


## ❓ FAQ

**Q: How do I calculate my available investment capital?**
You can use the `calculate_deployment_capacity` tool. Provide the total fund size, management fee rate, number of portfolio companies, and the follow-on allocation per company.

**Q: Can I simulate different exit outcomes?**
Yes, the `project_return_scenarios` tool allows you to input multiple exit multipliers to see how different success levels impact investor returns and manager carry.

**Q: How does recycling affect my fund?**
The `model_recycling_impact` tool calculates the incremental capital gain achieved by reinvesting realized gains from successful exits back into the fund.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-follow-on-fund-modeler](https://vinkius.com/ai-agent-connect/accelerator-follow-on-fund-modeler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Follow-on Fund Modeler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-follow-on-fund-modeler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Follow-on Fund Modeler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-follow-on-fund-modeler": {
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
