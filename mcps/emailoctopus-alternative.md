# EmailOctopus MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emailoctopus-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Send beautiful email campaigns at a fraction of the cost with a platform built for startups and growing businesses.

## Description
Connect your **EmailOctopus** (v2) account to any AI agent and take full control of your email marketing and subscriber engagement workflows through natural conversation.

### What you can do

- **Audience Orchestration** — List and manage your email marketing lists programmatically, including creating new lists and monitoring subscriber counts
- **Subscriber Lifecycle** — Programmatically add, update, or remove subscribers from lists and manage detailed profiles, tags, and custom fields
- **Campaign Management** — Monitor sent and draft campaigns and retrieve high-fidelity performance reports including open and click rates
- **Workflow Automation** — Programmatically trigger automated sequences (workflows) for specific contacts to coordinate complex customer journeys
- **Operational Visibility** — Retrieve complete list metadata and individual contact details directly through your agent for instant marketing reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your EmailOctopus settings (Integrations > API)
3. Start managing your marketing lists and campaigns from Claude, Cursor, or any MCP client

No more manual scrubbing through subscriber exports or slow UI navigation. Your AI acts as your dedicated email marketing and automation coordinator.

### Who is this for?

- **Marketing Managers** — instantly retrieve campaign results and update subscriber segments using natural language commands
- **Growth Marketers** — automate lead ingestion and trigger onboarding sequences without leaving your workspace
- **Business Owners** — monitor audience growth and manage subscriber lists through simple AI queries


## Available Tools (12)
- **add_contact_to_list**: Add a new contact to a list
- **create_email_list**: Create a new subscriber list
- **remove_contact_from_list**: Delete a contact from a list
- **get_campaign_details**: Get details for a campaign
- **get_contact_details**: Get details for a contact
- **get_list_details**: Get details for an email list
- **get_campaign_summary_report**: Get performance metrics for a campaign
- **list_email_campaigns**: List all sent and draft campaigns
- **list_contacts_in_list**: Can filter by status.

List contacts in a specific list
- **list_email_lists**: List all subscriber lists
- **trigger_automation_for_contact**: Requires API trigger to be enabled.

Start an automation for a contact
- **update_contact_profile**: Update an existing contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EmailOctopus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my email subscriber lists in EmailOctopus."

**🤖 AI Agent:**
> I've retrieved your email marketing lists. You have 3 active lists: 'Weekly Newsletter' (ID: l_123), 'Product Updates' (ID: l_456), and 'Lead Magnet'. Which one should we manage?

---

**👤 You:**
> "Add subscriber 'john.doe@example.com' to list 'l_123' with tag 'Customer'."

**🤖 AI Agent:**
> Done! John Doe has been successfully added to the 'Weekly Newsletter' list (ID: l_123) and tagged as a 'Customer'. Your team can now track their engagement in the dashboard.

---

**👤 You:**
> "Show me the report summary for campaign ID 'c_987'."

**🤖 AI Agent:**
> Fetching report... Campaign c_987 ('Spring Promo') has a 22% open rate and a 4% click-through rate so far. Total successful deliveries: 1,200. Shall I check for any bounced addresses?


## ❓ FAQ

**Q: How do I find my EmailOctopus API Key?**
Log in to your account, navigate to **Integrations** > **API**, and click **Create Key** to generate your unique access token.

**Q: Can I update custom fields for a contact?**
Yes! The `update_contact_profile` tool allows you to modify tags and any custom data fields associated with a subscriber.

**Q: How do I check the performance of a sent campaign?**
Use the `get_campaign_summary_report` tool with a campaign ID to retrieve real-time metrics including open and click rates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emailoctopus-alternative](https://vinkius.com/mcp/emailoctopus-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EmailOctopus** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emailoctopus-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EmailOctopus** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emailoctopus-alternative": {
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
