# Donately MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/donately)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [payment-processing](../categories/payment-processing.md)

Equip your AI agent to manage donations, track donors, and monitor fundraising campaigns via the Donately API.

## Description
Integrate **Donately**, the simplest online fundraising platform, directly into your AI workflow. Manage your donations and recurring contributions, track donor profiles and lifetime giving, monitor fundraising campaigns and progress, and oversee your fundraisers using natural language.

### What you can do

- **Donation Oversight** — List and retrieve detailed information and payment status for all your received contributions.
- **Donor Intelligence** — Monitor real-time donor profiles, contact details, and lifetime giving history across your organization.
- **Campaign Monitoring** — Track fundraising campaigns, goals, and current progress metrics to ensure successful outcomes.
- **Contribution Auditing** — Retrieve high-level summaries of fundraising performance and identify your most impactful contributors instantly.

### How it works

1. Connect the Donately integration to your AI assistant.
2. Authorize using your Donately API Key (found in your account settings).
3. Orchestrate your fundraising operations and donor relations through intuitive conversation.

### Who is this for?

- **Non-Profit Managers** — Quickly check campaign progress and recent donations on the go.
- **Development Officers** — Research donor history and lifetime giving via chat during outreach.
- **Operations Teams** — Monitor donation volumes and organizational fundraising metadata instantly.


## Available Tools (10)
- **get_donately_account_metadata**: Retrieve metadata and limits for your Donately account
- **get_campaign_performance_summary**: Retrieve a high-level summary of a specific campaigns performance
- **get_donation_details**: Get detailed information for a specific donation
- **get_donor_profile**: Get full profile and giving history for a specific donor
- **list_fundraising_campaigns**: List all fundraising campaigns configured in Donately
- **list_all_donations**: List all donations received in your Donately account
- **list_active_donors**: List all donors registered in your Donately organization
- **list_latest_contributions**: Identify the most recently received donations
- **list_highest_lifetime_donors**: Identify donors with the highest lifetime contribution totals (mock logic)
- **search_donations_by_email**: Search for donations matching a specific donor email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Donately** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the latest donations received."

**🤖 AI Agent:**
> I've found 5 recent donations, including $50.00 from 'John Doe' and $100.00 from 'Jane Smith'. All were successfully processed. Would you like to see the associated campaign for any of these?

---

**👤 You:**
> "Show me the progress for our 'Summer Relief' campaign."

**🤖 AI Agent:**
> The 'Summer Relief' campaign has raised $8,500 towards its $10,000 goal (85% complete). There have been 45 unique donors so far. Should I list the top contributors for this campaign?

---

**👤 You:**
> "Research the donor profile for 'robert.brown@example.com'."

**🤖 AI Agent:**
> Robert Brown is a regular donor with a lifetime total of $1,250.00 across 12 donations. Their last contribution was $100.00 on March 15th. Would you like to see their complete giving history?


## ❓ FAQ

**Q: How do I get a Donately API Key?**
Log in to your Donately dashboard, navigate to **Settings > API Key**, and you can retrieve your unique API Key from there. Ensure you have the necessary permissions within your organization.

**Q: Can the agent process new donations?**
This integration currently focuses on listing and auditing donations, donors, and campaigns. Processing new donations with credit card details should be managed via your Donately forms or donation pages.

**Q: Does the integration show recurring donations?**
Yes, you can use the list_all_donations or get_donation_details tools to identify and retrieve information for both one-time and recurring contributions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/donately](https://vinkius.com/mcp/donately)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Donately** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `donately` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Donately** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "donately": {
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
