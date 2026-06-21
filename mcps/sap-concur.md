# SAP Concur MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sap-concur)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Enable your AI agent to manage corporate expenses, track report statuses, and retrieve user profiles via the SAP Concur API.

## Description
Connect your AI assistant to **SAP Concur**, the leading platform for expense management, travel, and invoice automation.

### What you can do

- **Expense Tracking** — List and inspect individual expenses including amounts, categories, and receipt metadata.
- **Report Status** — Check approval status of any expense report.
- **User Profiles** — Retrieve employee profile data including cost center and department.

### How it works

1. Add the SAP Concur integration.
2. Register an app in the SAP Concur Developer Portal and provide the Client ID, Client Secret, and Refresh Token.
3. Query expense data via natural language commands.

### Who is this for?

- **Finance Teams** — Pull expense summaries without logging into the dashboard.
- **Travel Managers** — Verify travel policy compliance in real time.
- **Employees** — Check approval status of their own reports from chat.


## Available Tools (9)
- **get_expense**: Retrieve detailed information about a specific expense
- **list_pending_expenses**: Quickly list all expenses that have not yet been assigned to a report
- **get_expense_report**: Retrieve detailed information about a specific expense report
- **get_report_summaries**: Calculate basic totals for a list of recent expense reports
- **get_user_profile**: Retrieve the profile details of the currently authenticated Concur user
- **list_attendees**: Retrieve a list of expense attendees (for business meals, etc.)
- **list_expense_types**: Retrieve a list of valid expense types configured in your organization
- **list_expenses**: Retrieve a list of your expenses from Concur
- **list_expense_reports**: Retrieve a list of your expense reports from Concur


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SAP Concur** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my last 10 expenses in Concur."

**🤖 AI Agent:**
> Here are your 10 most recent expenses:
1. Uber ride — $24.50 (Jan 22)
2. Hotel — $189.00 (Jan 20)
3. Lunch meeting — $47.80 (Jan 18)
Would you like the full report for any of these?

---

**👤 You:**
> "Get the status of expense report 'rep-8842'."

**🤖 AI Agent:**
> Report 'rep-8842' is **Pending Approval**. Submitted by John Smith on Jan 20 with 5 entries totaling $412.30. Approver: Sarah Wilson.

---

**👤 You:**
> "Retrieve the profile for employee 'E-4545'."

**🤖 AI Agent:**
> Employee Profile:
- Name: Michael Davis
- ID: E-4545
- Department: Sales
- Cost Center: NA-West (CC-102)
- Manager ID: E-3300


## ❓ FAQ

**Q: How do I get my Concur Client ID and Secret?**
Register a new application in the SAP Concur Developer Portal. Once approved, you'll receive a Client ID and Client Secret.

**Q: What is the Refresh Token used for?**
SAP Concur uses OAuth 2.0. The Refresh Token automatically generates short-lived access tokens without requiring manual login each time.

**Q: Can I submit an expense report via this integration?**
The current version focuses on reading and listing data. Submit and approve capabilities may be added in future updates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sap-concur](https://vinkius.com/mcp/sap-concur)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SAP Concur** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sap-concur` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SAP Concur** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sap-concur": {
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
