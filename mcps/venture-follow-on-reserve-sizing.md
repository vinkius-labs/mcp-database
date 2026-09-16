# Venture Follow-on Reserve Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-follow-on-reserve-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate optimal capital reserves for venture capital follow-on investments.

## Description
This MCP server provides specialized financial modeling tools for venture capital firms to manage follow-on capital. It allows users to calculate the optimal reserve ratio, project annual deployment schedules, and reallocate reserves based on company performance tiers. Use `calculate_reserve_summary` to determine the initial vs. reserve split, `project_deployment_schedule` to plan capital over time, `allocate_by_performance_tier` to prioritize high-growth companies, and `validate_reserve_adequacy` to check if current reserves meet projected needs.


## Available Tools (4)
- **validate_reserve_adequacy**: Compares the calculated reserves against the expected follow-on needs
- **allocate_by_performance_tier**: g., high, medium, low).

Reallocates the total reserve based on the projected performance of portfolio companies
- **calculate_reserve_summary**: Provides a high-level overview of the fund's allocation between initial investments and reserves
- **project_deployment_schedule**: Determines how the reserves should be distributed over time across the portfolio


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Follow-on Reserve Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reserve summary for a $100M fund with a 60% initial investment ratio and 20 portfolio companies."

**🤖 AI Agent:**
> For a $100M fund with a 60% initial investment ratio, the initial investment amount is $60M and the total reserve amount is $40M. The optimal reserve ratio is 40%, and the reserve per company is $2M.

---

**👤 You:**
> "Project a deployment schedule for $40M in reserves over 5 years for 20 companies."

**🤖 AI Agent:**
> The annual reserve allocation for the 5-year period is $8,000,000 per year, totaling $40,000,000.

---

**👤 You:**
> "Is a $30M reserve adequate for expected follow-on needs of $35M?"

**🤖 AI Agent:**
> No, the reserves are not adequate. There is a shortfall of $5,000,000.


## ❓ FAQ

**Q: How do I calculate the reserve per company?**
You can use the `calculate_reserve_summary` tool, which takes the fund size, initial investment ratio, and portfolio company count to return the average reserve available per company.

**Q: Can I prioritize certain companies for follow-on funding?**
Yes, the `allocate_by_performance_tier` tool allows you to distribute reserves based on performance categories like high, medium, or low priority.

**Q: How can I check if my reserves are sufficient?**
Use the `validate_reserve_adequacy` tool to compare your total available reserves against your expected follow-on needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-follow-on-reserve-sizing](https://vinkius.com/en/ai-agent-connect/venture-follow-on-reserve-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Follow-on Reserve Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-follow-on-reserve-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Follow-on Reserve Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-follow-on-reserve-sizing": {
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
