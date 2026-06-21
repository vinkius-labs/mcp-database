# DAS Payment Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/das-payment-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automated annual calendar generator for Brazilian Simples Nacional tax payments, handling holiday-based date shifts and overdue period alerts.

## Description
The DAS Payment Scheduler is a specialized tool for Brazilian entrepreneurs to manage their Simples Nacional tax obligations. It automatically calculates the exact payment deadlines by checking if the standard 20th of the month falls on a weekend or a national holiday, shifting the date forward to the next business day when necessary. Using `generate_annual_schedule`, you can view your entire year's payment plan at once. If you are unsure why a specific date changed, use `inspect_holiday_impact` to see the reason for the shift. Additionally, the `identify_overdue_periods` tool helps you stay on top of your taxes by alerting you to any months where the deadline has already passed.


## Available Tools
- **generate_annual_schedule**: Generates a yearly schedule of DAS payments
- **inspect_holiday_impact**: Inspects if a specific payment date was moved due to holidays or weekends
- **identify_overdue_periods**: Identifies which months have passed their DAS payment deadline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DAS Payment Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my DAS payment schedule for 2024."

**🤖 AI Agent:**
> Here is your DAS payment schedule for 2024. The first payment (competence January) is due on 2024-02-20, and all subsequent months follow the standard 20th rule unless adjusted for holidays.

---

**👤 You:**
> "Are there any overdue DAS payments as of today (2024-05-15)?"

**🤖 AI Agent:**
> As of 2024-05-15, the following periods are overdue: January (deadline was 2024-02-20), February (deadline was 2024-03-20), and March (deadline was 2024-04-20).

---

**👤 You:**
> "Why was the May 20th payment date moved in 2024?"

**🤖 AI Agent:**
> The payment for May 2024 remains on 2024-05-20 as there are no national holidays or weekends interfering with this specific date.


## ❓ FAQ

**Q: How does the tool handle holidays?**
If the 20th of the month falls on a weekend or a Brazilian national holiday, the tool automatically shifts the due date to the next available business day.

**Q: Can I see my entire year at once?**
Yes, by using the `generate_annual_schedule` tool and providing the desired year.

**Q: How do I know if I missed a payment?**
You can use the `identify_overdue_periods` tool with a reference date to see all months where the deadline has already passed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/das-payment-scheduler](https://vinkius.com/mcp/das-payment-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DAS Payment Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `das-payment-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DAS Payment Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "das-payment-scheduler": {
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
