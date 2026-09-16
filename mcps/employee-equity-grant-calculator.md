# Employee Equity Grant Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/employee-equity-grant-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate standardized equity grant recommendations based on seniority, experience, and company stage.

## Description
This MCP server provides a standardized framework for calculating employee equity grants. It balances internal fairness with market competitiveness by analyzing role levels, professional experience, and the company's current lifecycle stage. Use `get_recommended_grant` to determine the ideal equity percentage, `get_vesting_schedule` to generate ownership timelines, and `get_exercise_window` to define post-separation rights. It also includes `validate_pool_availability` to ensure proposed grants remain within the company's remaining option pool.


## Available Tools (4)
- **get_vesting_schedule**: Provides the timeline for equity ownership
- **get_exercise_window**: Defines the period during which an employee can exercise options after separation
- **get_recommended_grant**: Determines the specific equity percentage recommended for a new hire
- **validate_pool_availability**: Checks if a proposed grant is feasible given the current company resources


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Employee Equity Grant Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the recommended equity grant for a Senior-Level engineer with 8 years of experience at a Seed stage company?"

**🤖 AI Agent:**
> The recommended equity grant for a Senior-Level engineer with 8 years of experience at a Seed stage company is 0.45%.

---

**👤 You:**
> "Generate a vesting schedule for a 0.5% grant with a 48-month retention target."

**🤖 AI Agent:**
> The 0.5% grant will vest over 48 months, with 0.0104% allocated each month.

---

**👤 You:**
> "How long is the exercise window for a Director-Level employee?"

**🤖 AI Agent:**
> A Director-Level employee has an exercise window of 120 months.


## ❓ FAQ

**Q: How is the recommended grant calculated?**
The grant is calculated by intersecting the role level with the company stage, then adjusting for years of experience and adding a premium for critical roles via `get_recommended_grant`.

**Q: Can I check if a grant fits within my company's budget?**
Yes, you can use the `validate_pool_availability` tool to compare a proposed grant against the remaining option pool percentage.

**Q: What determines the vesting period?**
The vesting period is determined by the desired retention target months provided to the `get_vesting_schedule` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/employee-equity-grant-calculator](https://vinkius.com/en/ai-agent-connect/employee-equity-grant-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Employee Equity Grant Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `employee-equity-grant-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Employee Equity Grant Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "employee-equity-grant-calculator": {
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
