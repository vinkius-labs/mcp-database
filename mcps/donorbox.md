# Donorbox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/donorbox)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [payment-processing](../categories/payment-processing.md)

Equip your AI agent to manage donations, track recurring plans, and monitor fundraising campaigns via the Donorbox API.

## Description
Integrate **Donorbox**, the powerful and easy-to-use donation software, directly into your AI workflow. Manage your one-time and recurring donations, track donor profiles and subscription plans, monitor fundraising campaigns and progress, and oversee your donation forms using natural language.

### What you can do

- **Donation Oversight** — List and retrieve detailed information and payment status for all your received contributions.
- **Subscription Intelligence** — Monitor active recurring donation plans, frequencies, and donor identifiers across your organization.
- **Campaign Monitoring** — Track fundraising campaigns, goals, total raised amounts, and progress percentages to ensure successful outcomes.
- **Donor Auditing** — Retrieve high-level summaries of donor engagement and identify your most loyal contributors instantly.

### How it works

1. Connect the Donorbox integration to your AI assistant.
2. Authorize using your Donorbox account email and API Key.
3. Orchestrate your fundraising operations and donor management through intuitive conversation.

### Who is this for?

- **Fundraising Managers** — Quickly check campaign goals and recent contribution volumes on the go.
- **Non-Profit Administrators** — Research donor history and recurring plan statuses via chat.
- **Finance Teams** — Monitor donation amounts and campaign success rates across the organization instantly.


## Available Tools (10)
- **get_donorbox_account_metadata**: Retrieve metadata for the current authenticated user
- **get_campaign_details**: Get detailed settings and progress for a specific campaign
- **quick_campaign_performance_audit**: Retrieve a high-level summary of all campaign success rates
- **list_active_subscription_plans**: Identify recurring plans that are currently in an "Active" status
- **list_fundraising_campaigns**: List all fundraising campaigns configured in Donorbox
- **list_donorbox_donations**: List all donations received in your Donorbox account
- **list_registered_donors**: List all donors registered in your Donorbox organization
- **list_latest_contributions**: Identify the most recently received donations
- **list_recurring_donation_plans**: List all active recurring donation plans
- **search_donors_by_email**: Search for a donor using their email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Donorbox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recent donations received in Donorbox."

**🤖 AI Agent:**
> I've found 5 recent donations, including $25.00 from 'Alice Johnson' and $100.00 from 'Michael Smith'. All are marked as 'Completed'. Would you like to see which campaign they supported?

---

**👤 You:**
> "Show me the performance for campaign 'Save the Oceans'."

**🤖 AI Agent:**
> The 'Save the Oceans' campaign has raised $12,450 towards its $15,000 goal (83% reached). There are currently 12 active recurring donors for this campaign. Should I pull the list of recent contributions?

---

**👤 You:**
> "Find the recurring plan for donor 'sarah.jones@example.org'."

**🤖 AI Agent:**
> Sarah Jones has an active monthly recurring plan of $50.00 that started on January 1st. They have made 3 successful payments to date. Would you like me to check their next scheduled donation date?


## ❓ FAQ

**Q: How do I get a Donorbox API Key?**
Log in to your Donorbox account, navigate to **Account > API & Integrations**, and you can generate or retrieve your unique API Key from there. You will also need your account email.

**Q: Can the agent manage recurring plans?**
This integration currently focuses on listing and auditing recurring plans and their status. Modifying plan details or amounts should be managed via the Donorbox dashboard.

**Q: Does the integration show donor contact info?**
Yes, you can use the list_registered_donors or search_donors_by_email tools to retrieve donor profile details, including their registered email addresses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/donorbox](https://vinkius.com/mcp/donorbox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Donorbox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `donorbox` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Donorbox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "donorbox": {
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
