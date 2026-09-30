# Wedding Vendor Payment Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wedding-vendor-payment-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Transforms vendor contracts into structured payment timelines and budget trackers.

## Description
This MCP server manages wedding finances by converting vendor contracts into actionable payment schedules. Use `get_vendor_payment_schedule` to calculate specific deposit and installment dates, `check_budget_compliance` to ensure costs stay within category limits, `generate_master_payment_calendar` to see all upcoming payments in one view, and `calculate_cash_flow_forecast` to project total spending at specific milestones.


## Available Tools (4)
- **calculate_cash_flow_forecast**: Projects total wedding expenditure at a specific milestone date
- **check_budget_compliance**: Determines if a vendor contract fits within the predefined budget for its category
- **generate_master_payment_calendar**: Creates a unified, chronological list of all upcoming payments for all vendors
- **get_vendor_payment_schedule**: Calculates specific payment dates and amounts for a single vendor


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wedding Vendor Payment Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the payment schedule for 'Floral Designs' with a total contract of $2000, a $500 deposit due on 2024-05-01, and installments due on 2024-07-01 and 2024-09-01."

**🤖 AI Agent:**
> The payment schedule for Floral Designs is: $500 deposit on 2024-05-01, $750 installment on 2024-07-01, and $750 installment on 2024-09-01.

---

**👤 You:**
> "Is a $3500 catering contract within my $3000 catering budget?"

**🤖 AI Agent:**
> No, the catering contract is over budget by $500.

---

**👤 You:**
> "What will my total wedding expenditure be by 2024-12-31?"

**🤖 AI Agent:**
> The total expenditure projected by 2024-12-31 is $5,250.


## ❓ FAQ

**Q: How do I calculate my vendor's payment dates?**
You can use the `get_vendor_payment_schedule` tool by providing the vendor name, total contract value, deposit amount, deposit date, and a list of installment dates.

**Q: Can I check if I am over my wedding budget?**
Yes, use `check_budget_compliance` to compare a vendor's contract value against your allocated budget for that specific category.

**Q: How can I see all my upcoming payments at once?**
The `generate_master_payment_calendar` tool creates a single chronological list of all deposits and installments from all your vendor schedules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wedding-vendor-payment-planner](https://vinkius.com/en/ai-agent-connect/wedding-vendor-payment-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wedding Vendor Payment Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wedding-vendor-payment-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wedding Vendor Payment Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wedding-vendor-payment-planner": {
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
