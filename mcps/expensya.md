# Expensya MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/expensya)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Submit and approve business expenses in seconds with receipt scanning, policy enforcement, and reimbursement workflows.

## Description
Connect your **Expensya** account to any AI agent and take full control of your business spending and automated expense reporting through natural conversation.

### What you can do

- **Expense Orchestration** — List and manage all business expenses programmatically, including retrieving detailed metadata and creating new entries with comments
- **Report Oversight** — Monitor the status of expense reports (Draft, Pending Approval) and access project allocations for high-fidelity financial tracking
- **Organizational Visibility** — Retrieve complete directories of users, categories, and payment methods to coordinate team-wide spending policies
- **Logistics Intelligence** — List and manage vehicles for mileage tracking and monitor supported currencies for international business operations
- **Financial Export** — Programmatically trigger exports of expense data using predefined Export IDs for seamless integration with your accounting tools

### How it works

1. Subscribe to this server
2. Retrieve your **Expensya Token** (Administration > Integrations > API Keys)
3. Obtain your **Ocp-Apim-Subscription-Key** from the Expensya Developer Portal
4. Start managing your expenses from Claude, Cursor, or any MCP client

No more manual entry of every coffee receipt. Your AI acts as your dedicated finance and expense coordinator.

### Who is this for?

- **Finance Teams** — instantly retrieve organizational spending reports and monitor approval queues using natural language
- **Business Travelers** — quickly log new expenses and check project budgets without opening the web dashboard
- **Accountants** — automate the extraction of financial records and audit mileage logs through simple AI queries


## Available Tools
- **create_new_expense**: Requires amount, currency, and category.

Add a new expense record
- **export_expense_data**: Export expenses to a specific format
- **get_authenticated_user_profile**: Get current user profile
- **list_expense_categories**: g., Meals, Travel).

List active expense categories
- **list_supported_currencies**: List all supported currencies
- **list_expenses**: Supports filtering by date, user, and status.

List all business expenses
- **list_payment_methods**: g., Cash, Company Card) configured.

List defined payment methods
- **list_analytical_projects**: List projects for tracking
- **list_expense_reports**: List expense reports (folders)
- **list_expense_tags**: List active tags
- **list_expensya_users**: List users in the organization
- **list_mileage_vehicles**: List vehicles for mileage tracking


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Expensya** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my expenses from the last week."

**🤖 AI Agent:**
> I've retrieved 4 expenses from the last 7 days, including 'Dinner with Client' (€65.00) and 'Taxi to Airport' (€25.00). Would you like the full details for any of these?

---

**👤 You:**
> "Create a new expense: €12.50 for 'Office Supplies' with comment 'New notebook'."

**🤖 AI Agent:**
> Done! I've registered the €12.50 expense for 'Office Supplies'. It's now added to your dashboard for reconciliation. Shall I check your current total for this category?

---

**👤 You:**
> "Show me the status of my pending expense reports."

**🤖 AI Agent:**
> Checking reports... You have 2 reports currently 'Pending Approval'. One is from the 'Paris Business Trip' and the other is 'Monthly Expenses June'. I can provide the individual line items if needed.


## ❓ FAQ

**Q: How do I find my Expensya Token?**
Log in to Expensya as an admin, navigate to **Administration** > **Integrations** > **API Keys**, and generate your unique token.

**Q: What is the Ocp-Apim-Subscription-Key?**
This is an additional security key obtained by registering on the [**Expensya Developer Portal**](https://developer.expensya.com/) and subscribing to an API product.

**Q: Can I automate exports through the agent?**
Yes! Use the `export_expense_data` tool and provide a valid `exportId`. The agent will trigger the export process in the background.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/expensya](https://vinkius.com/mcp/expensya)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Expensya** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `expensya` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Expensya** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "expensya": {
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
