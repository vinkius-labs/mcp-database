# Constant Contact MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/constant-contact-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage your email marketing and contacts via Constant Contact — create campaigns, track engagement, and organize lists directly from your AI agent.

## Description
Connect your **Constant Contact** account to any AI agent to streamline your marketing automation and audience management through natural language.

### What you can do

- **Contact Management** — Create, update, and delete contacts, or manage list memberships and tags in bulk.
- **Campaign Orchestration** — Create, schedule, and test email campaigns directly from your conversation.
- **Deep Analytics** — Retrieve engagement rates, opens, clicks, and bounces to understand your campaign performance.
- **Account Insights** — Access account summaries and user privileges to ensure your integration is running smoothly.

### How it works

1. Subscribe to this server
2. Enter your Constant Contact Access Token
3. Start managing your marketing workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketers** — quickly check campaign stats and manage lists without switching tabs.
- **Sales Teams** — add new leads to specific segments and track engagement in real-time.
- **Business Owners** — automate routine marketing tasks and get instant reports on audience growth.


## Available Tools
- **add_list_memberships**: Bulk add contacts to lists
- **add_tags_to_contacts**: Bulk add tags to contacts
- **bulk_delete_contacts**: Bulk delete contacts
- **create_campaign**: Create a new email campaign
- **create_contact**: Create a new contact
- **create_list**: Create a new contact list
- **create_segment**: Create a new segment
- **create_tag**: Create a new contact tag
- **delete_contact**: Soft delete a contact
- **delete_list**: Delete a contact list
- **delete_segment**: Delete a segment
- **export_contacts**: Bulk export contacts to CSV
- **get_account_summary**: Get Constant Contact account summary
- **get_activity_status**: Check the status of a bulk activity
- **get_campaign_bounces**: Get tracking report for campaign bounces
- **get_campaign_clicks**: Get tracking report for campaign clicks
- **get_campaign_details**: Get details for a specific email campaign
- **get_campaign_opens**: Get tracking report for campaign opens
- **get_campaign_optouts**: Get tracking report for campaign opt-outs
- **get_campaign_sends**: Get tracking report for campaign sends
- **get_contact_activity_details**: Get activity details for a specific contact
- **get_contact_activity_summary**: Get activity summary for a specific contact
- **get_contact_engagement_rates**: Get open and click rates for a specific contact
- **get_contacts**: Get contacts with optional filtering
- **get_email_campaign_summaries**: Get summary reports for email campaigns
- **get_lists**: Get all contact lists
- **get_segments**: Get all segments
- **get_tags**: Get all contact tags
- **get_user_privileges**: Get user privileges for the current token
- **import_contacts_json**: Bulk import contacts via JSON
- **schedule_campaign**: Schedule an email campaign to send
- **sign_up_form**: Create or update a contact via sign up form
- **test_campaign**: Send a test email for a campaign
- **update_account_summary**: Requires state_code if country is US or CA.

Update Constant Contact account summary
- **update_campaign_activity**: Update a campaign activity (e.g., add lists/segments before sending)
- **update_contact**: Update an existing contact
- **update_list**: Update an existing contact list


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Constant Contact** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my contact lists in Constant Contact."

**🤖 AI Agent:**
> I've retrieved your lists. You have 3 active lists: 'Newsletter Subscribers' (ID: 101), 'VIP Customers' (ID: 102), and 'Event Leads' (ID: 103).

---

**👤 You:**
> "Show me the engagement rates for my contacts."

**🤖 AI Agent:**
> Fetching engagement data... Your overall engagement rates show a 24% open rate and a 3.5% click-through rate across your recent campaigns.

---

**👤 You:**
> "Get the details for campaign ID 12345."

**🤖 AI Agent:**
> Inspecting campaign 12345... This is the 'Summer Sale' email. It was sent to 1,200 recipients and is currently in 'Scheduled' status for tomorrow morning.


## ❓ FAQ

**Q: Can I see how many people opened my last email campaign?**
Yes! Use the `get_campaign_opens` tool with your campaign ID. Your agent will return the list of contacts who opened the email along with timestamps.

**Q: How do I check what permissions my current API token has?**
Simply ask the agent to run the `get_user_privileges` action. It will list all authorized scopes and privileges associated with your connected account.

**Q: Can I get a high-level overview of my account details?**
Yes, the `get_account_summary` tool provides organization names, contact information, and other core account metadata in a single query.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/constant-contact-alternative](https://vinkius.com/mcp/constant-contact-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Constant Contact** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `constant-contact-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Constant Contact** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "constant-contact-alternative": {
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
