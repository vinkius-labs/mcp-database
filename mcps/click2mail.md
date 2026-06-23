# Click2Mail MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/click2mail)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage physical mail and printing via Click2Mail — track jobs, monitor credit balance, and submit mailings directly from any AI agent.

## Description
Connect your **Click2Mail** account to any AI agent and take full control of your physical mailing and printing operations through natural conversation. Streamline how you manage letters, postcards, and certified mail natively.

### What you can do

- **Job Oversight** — List and retrieve details for all physical mail printing and mailing jobs natively
- **Cost Intelligence** — Access estimated costs for mail jobs before submission to manage budgets flawlessly
- **Asset Logistics** — List uploaded documents and address lists available for your mailing campaigns securely
- **Order Automation** — Submit mail jobs for production and delivery directly from your chat interface flawlessly
- **Credit Tracking** — Retrieve your current account credit balance for mailing flawlessly
- **Activity Auditing** — Access a history of account activities and transactions directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Click2Mail Username and Password
3. Start managing your physical mail from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — automate physical mail workflows and verify job statuses using natural language
- **Marketing Teams** — audit direct mail campaign costs and asset availability without opening the dashboard
- **Finance Teams** — quickly look up transaction history and credit balances straight from their chat interface
- **Customer Support** — verify status of certified mail and individual recipient deliveries


## Available Tools (8)
- **get_mail_credit_balance**: Retrieve the current account credit balance for mailing
- **get_mail_job_cost**: Retrieve the estimated cost for a mail job before submission
- **get_mail_job_details**: Get detailed information for a specific mail job
- **get_mail_account_history**: Retrieve a history of account activities and transactions
- **list_mail_address_lists**: List uploaded address lists available for mailing
- **list_mail_documents**: List uploaded documents available for mailing
- **list_mail_jobs**: List all physical mail printing and mailing jobs
- **submit_mail_job**: Submit a mail job for production and delivery


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Click2Mail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active mail jobs in Click2Mail."

**🤖 AI Agent:**
> Retrieving your mail jobs... I found 3 items: 'Monthly Invoices' (In Production), 'New Year Postcards' (Mailed), and 'Service Notice' (Pending). Would you like the tracking for the postcards?

---

**👤 You:**
> "What is the cost for job ID 98765?"

**🤖 AI Agent:**
> Checking cost for job 98765... The total estimated cost is $42.50 ($12.50 for printing and $30.00 for postage). You have enough credit to submit this job.

---

**👤 You:**
> "Show me my current mailing credit balance."

**🤖 AI Agent:**
> Checking account balance... You currently have $150.75 in mailing credits available. This can be used for any future physical mailing jobs.


## ❓ FAQ

**Q: Can I check the cost of a mailing before I send it?**
Yes! Use the `get_mail_job_cost` tool with the job ID. The agent will return the estimated production and postage costs for your mailing.

**Q: How do I see if my documents have been printed and mailed?**
Use the `get_mail_job_details` tool. Your agent will fetch the current production status (e.g., In Production, Mailed) and provide tracking info if available.

**Q: Where do I find my Click2Mail API credentials?**
Click2Mail uses your standard account Username and Password for API access. You can find your account details in the Click2Mail portal under Profile.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/click2mail](https://vinkius.com/mcp/click2mail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Click2Mail** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `click2mail` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Click2Mail** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "click2mail": {
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
