# Accelerator Fund Sizing Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-fund-sizing-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate optimal accelerator fund sizes, deployment velocity, and reserve adequacy.

## Description
This MCP server provides specialized financial modeling tools for venture capital and accelerator managers. It allows AI agents to determine the total capital required for a fund by analyzing cohort frequency, investment per company, and management fees. Use `get_fund_sizing_summary` to get a full capital allocation breakdown, `get_deployment_velocity` to plan annual capital needs, and `get_reserve_adequacy_check` to ensure follow-on reserves are sufficient for the planned number of companies.


## Available Tools (3)
- **get_deployment_velocity**: Calculates the annual capital requirements to ensure the fund can sustain its planned pace
- **get_fund_sizing_summary**: Provides a complete breakdown of the fund's capital allocation and deployment capacity
- **get_reserve_adequacy_check**: Validates if the current fund structure provides enough follow-on capacity relative to the total number of companies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Fund Sizing Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total fund size for an accelerator with 2 cohorts per year, 10 companies per cohort, $100,000 investment per company, 20% follow-on reserve, 2% annual management fee, and a 5-year duration."

**🤖 AI Agent:**
> The total fund size required is $1,500,000. This includes $1,000,000 for initial investments, $200,000 for follow-on capacity, and $150,000 for management fees over 5 years, with remaining capital accounting for the fund structure.

---

**👤 You:**
> "What is the annual deployment requirement for a fund with 4 cohorts per year, 5 companies per cohort, and $50,000 investment per company?"

**🤖 AI Agent:**
> The annual deployment requirement is $100,000.

---

**👤 You:**
> "Check if a fund with $5,000,000 total size, $4,000,000 deployable capital, 10% follow-on reserve, and 100 companies has sufficient reserves."

**🤖 AI Agent:**
> The follow-on capacity per company is $40,000, and the reserve is sufficient.


## ❓ FAQ

**Q: How do I calculate the total fund size needed?**
You can use the `get_fund_sizing_summary` tool. Provide the number of cohorts per year, companies per cohort, initial investment per company, follow-on reserve percentage, management fee percentage, and the fund duration.

**Q: Can I check if my follow-on reserves are enough?**
Yes, the `get_reserve_adequacy_check` tool validates if your current fund structure provides sufficient follow-on capacity relative to the total number of companies invested in.

**Q: How does this tool handle management fees?**
The management fee is calculated as an annual percentage of the total fund size and multiplied by the fund duration to determine the total fee budget.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-fund-sizing-model](https://vinkius.com/ai-agent-connect/accelerator-fund-sizing-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Fund Sizing Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-fund-sizing-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Fund Sizing Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-fund-sizing-model": {
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
