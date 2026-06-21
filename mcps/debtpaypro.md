# DebtPayPro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/debtpaypro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Equip your AI agent to manage contacts, track payments, and monitor sales opportunities via the DebtPayPro API.

## Description
Integrate **DebtPayPro**, the specialized CRM for the debt settlement and financial services industry, directly into your AI workflow. Manage your customer database, track scheduled payments and debt portfolios, and monitor sales opportunities using natural language.

### What you can do

- **Contact Management** — List and retrieve detailed profiles for your CRM contacts and leads.
- **Payment Tracking** — Monitor payment history and upcoming scheduled payments for specific clients.
- **Debt Portfolio Oversight** — List and review debts associated with your contacts.
- **Sales & Task Monitoring** — Track active sales opportunities and manage pending CRM tasks and follow-ups.

### How it works

1. Connect the DebtPayPro integration to your AI assistant.
2. Authorize using your DebtPayPro API Key (found in your admin settings).
3. Optimize your debt settlement operations through intuitive conversation.

### Who is this for?

- **Debt Settlement Agents** — Quickly check client balances and payment statuses on the go.
- **Compliance Officers** — Audit contact profiles and debt records via chat.
- **Sales Managers** — Monitor lead pipelines and team task completion during planning.


## Available Tools
- **create_new_contact**: Persists a new contact record with the provided name and email, returning the newly generated system ID.

Add a new contact to the DebtPayPro database
- **get_account_details**: Returns account-level metadata such as company name, API permissions, and system version.

Retrieve metadata for your DebtPayPro account
- **get_contact_details**: Resolves demographic data, associated case numbers, and the current status of their debt settlement program.

Get detailed profile information for a specific contact
- **list_crm_contacts**: Returns contact metadata including system IDs, names, and primary contact information.

List all contacts in your DebtPayPro CRM
- **list_contact_debts**: Returns a list of enrolled debts, including creditor names, original balances, and current settlement status.

List all debts associated with a specific contact
- **list_sales_opportunities**: Returns a list of active opportunities including projected case value, current stage in the sales cycle, and assigned sales representative.

List active sales opportunities and leads
- **list_contact_payments**: Returns a history of processed payments and a schedule of future installments towards their debt settlement plan.

List payment history and scheduled payments for a contact
- **list_crm_tasks**: Returns task descriptions, due dates, and associated contact or case identifiers.

List pending tasks and follow-ups in the system
- **list_upcoming_payments**: Returns upcoming transaction metadata for proactive account management.

List payments scheduled for the next 7 days (mock logic)
- **search_contacts_by_name**: Matches the search term against names and email addresses using partial case-insensitive matching.

Search for a contact by name or email keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DebtPayPro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active contacts in the 'Settlement' stage."

**🤖 AI Agent:**
> I've found 8 contacts currently in the 'Settlement' stage, including 'Alice Johnson' and 'Bob Miller'. Their total enrolled debt is $45,000. Would you like to see their recent payment history?

---

**👤 You:**
> "Show me the debts associated with contact 'John Smith'."

**🤖 AI Agent:**
> John Smith has 3 enrolled debts: 'Chase Credit Card' ($5,000), 'Wells Fargo Loan' ($12,000), and 'Citi Bank Card' ($3,500). All are currently 'Active'. Should I check his scheduled payments for next month?

---

**👤 You:**
> "List all CRM tasks assigned to me for today."

**🤖 AI Agent:**
> You have 5 tasks assigned for today, including 3 'Follow-up Calls' and 2 'Document Reviews'. The highest priority is a call with 'Global Exports'. Should I pull their contact profile for you?


## ❓ FAQ

**Q: How do I get a DebtPayPro API Key?**
Log in to your DebtPayPro account, navigate to the API section in your settings (usually under **Admin > API**), and you can generate or retrieve your API Key from there.

**Q: Can the agent update payment schedules?**
This integration currently focuses on listing and retrieving contacts, debts, and payments for analysis. Modifying existing payment schedules should be managed via the DebtPayPro dashboard.

**Q: Does the integration support custom fields?**
Yes, standard contact and opportunity data, including common fields, are retrieved. If your plan includes API access to custom fields, they will be visible in the raw JSON response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/debtpaypro](https://vinkius.com/mcp/debtpaypro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DebtPayPro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `debtpaypro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DebtPayPro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "debtpaypro": {
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
