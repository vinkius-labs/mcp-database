# CaptivateIQ MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/captivateiq)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage incentive compensation via CaptivateIQ — track commission payouts, statements, and employee plans directly from any AI agent.

## Description
Connect your **CaptivateIQ** account to any AI agent and orchestrate your incentive compensation, commission tracking, and payroll integration workflows through natural conversation.

### What you can do

- **Payout Oversight** — List and retrieve detailed metadata for all processed commission payouts across your organization.
- **Statement Management** — Access individualized payout statements for employees to verify earnings and calculations.
- **Employee Coordination** — List and retrieve detailed profiles for all employees, including their plan designations and hierarchy.
- **Workbook Monitoring** — Access and list your calculation workbooks and worksheets to ensure transparency in your commission logic.
- **Dispute Tracking** — Monitor and list commission inquiries or disputes directly from your workspace.
- **Financial Reporting** — Retrieve core account and integration information straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your CaptivateIQ API Token
3. Start managing your commission data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance & Payroll Teams** — quickly extract payout data for payroll runs without manual dashboard exports.
- **Sales Operations** — monitor commission trends and employee designations straight from their workflow tools.
- **Revenue Leaders** — retrieve high-level payout summaries and plan details using natural language.


## Available Tools (8)
- **get_account_status**: Retrieve core account/integration information
- **get_employee_details**: Get details of a specific employee
- **list_employees**: List all employee records and plan designations
- **list_commission_inquiries**: List commission disputes and inquiries (generic search)
- **list_commission_payouts**: List all processed commission payouts
- **list_payout_statements**: List individualized payout statements for employees
- **list_workbooks**: List all calculation workbooks
- **list_worksheets**: List all calculation worksheets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CaptivateIQ** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all processed commission payouts in CaptivateIQ."

**🤖 AI Agent:**
> I've retrieved your payouts. You have several recent payouts, including 'March Sales Cycle' (Total: $120,000) and 'Q1 Bonus Run' (Total: $45,000).

---

**👤 You:**
> "Show the payout statement for employee John Doe."

**🤖 AI Agent:**
> Retrieving statement for John Doe... For the last period, he earned a total commission of $4,500 based on his sales target attainment of 110%.

---

**👤 You:**
> "Which calculation workbooks are available in my account?"

**🤖 AI Agent:**
> You have 3 active workbooks: 'Global Sales Plan 2026', 'Manager Incentive Tier', and 'Referral Program Logic'. Which one would you like to explore?


## ❓ FAQ

**Q: Can I check the total commission for a specific employee using the agent?**
Yes! Use the `get_employee_details` tool or the `list_payout_statements` tool. Your agent will fetch the relevant data, including the total commission amount for the period.

**Q: How do I list all the processed payouts for my team?**
Simply ask the agent to `list_commission_payouts`. It will retrieve the full history of processed payouts from your CaptivateIQ account, including dates and totals.

**Q: Does the integration allow creating a new payout manual adjustment?**
The current toolset focuses on querying and monitoring (Read-Only) for data analysis and payroll extraction. Adjustments or changes to the calculation logic should be managed via the CaptivateIQ web platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/captivateiq](https://vinkius.com/mcp/captivateiq)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CaptivateIQ** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `captivateiq` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CaptivateIQ** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "captivateiq": {
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
