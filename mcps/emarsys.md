# Emarsys MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emarsys)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage email campaigns, track contact lists, and monitor automation programs via the Emarsys API.

## Description
Integrate **Emarsys**, the comprehensive customer engagement platform, directly into your AI workflow. Manage your email marketing campaigns and contact lists, track audience segments and automation programs, monitor trigger events and registration forms, and oversee your omnichannel engagement using natural language.

### What you can do

- **Campaign Oversight** — List and retrieve detailed information, subject lines, and launch statuses for all your email campaigns.
- **Contact Intelligence** — Monitor marketing contact lists and audience segments, resolving structural details and filter criteria.
- **Automation Management** — Access and monitor automation programs and workflows, tracking active statuses and trigger events.
- **Engagement Auditing** — Retrieve high-level summaries of campaign volume, list activity, and organizational marketing health instantly.

### How it works

1. Connect the Emarsys integration to your AI assistant.
2. Authorize using your Emarsys API User and Secret Key (W-SSE authentication).
3. Orchestrate your customer engagement and marketing automation through intuitive conversation.

### Who is this for?

- **Marketing Managers** — Quickly check campaign launch statuses and audience sizes on the go.
- **CRM Specialists** — Research segments and automation workflows via chat during campaign planning.
- **Operations Teams** — Monitor marketing volumes and organizational Emarsys metadata instantly.


## Available Tools (10)
- **get_emarsys_account_metadata**: Retrieve metadata and settings for your Emarsys account
- **get_campaign_details**: Get detailed settings and status for a specific email campaign
- **get_contact_list_details**: Get detailed settings for a specific contact list
- **quick_engagement_volume_audit**: Retrieve a high-level summary of campaigns, lists, and automation programs
- **list_automation_programs**: List all automation programs and workflows
- **list_email_campaigns**: List all email campaigns in your Emarsys account
- **list_marketing_contact_lists**: List all contact lists configured in your organization
- **list_trigger_events**: List all external events used for triggering automation programs
- **list_registration_forms**: List all subscription and registration forms
- **list_audience_segments**: List all audience segments (filters) in your account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emarsys** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active email campaigns."

**🤖 AI Agent:**
> I've found several campaigns, including 'Summer Flash Sale' and 'Weekly Round-up'. The Summer Flash Sale is currently 'Launched' and was sent to 50,000 contacts. Would you like to see the details?

---

**👤 You:**
> "Show me the audience segments in my account."

**🤖 AI Agent:**
> I've retrieved your segments, including 'High-Value Customers' (1,200 contacts) and 'Recent Sign-ups' (5,500 contacts). Should I check the filter criteria for the High-Value segment?

---

**👤 You:**
> "What automation programs are currently running?"

**🤖 AI Agent:**
> You have 3 active automation programs: 'Welcome Journey', 'Abandoned Cart Recovery', and 'Post-Purchase Follow-up'. Should I pull the latest activity for the Abandoned Cart program?


## ❓ FAQ

**Q: How do I get Emarsys API credentials?**
Log in to your Emarsys account, navigate to **Admin > Web Services**, and you can create or retrieve your **API Username** and **Secret Key**. Ensure the user has the required permissions for the resources you wish to access.

**Q: What authentication method does this integration use?**
This integration uses **W-SSE authentication**, which is the standard for the Emarsys API. It requires both your API Username and Secret Key to securely generate request headers.

**Q: Can the agent trigger automation programs?**
This integration currently focuses on listing and auditing programs and events. Triggering specific automation workflows should be managed via external events in the Emarsys dashboard or dedicated transactional API calls.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emarsys](https://vinkius.com/mcp/emarsys)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emarsys** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emarsys` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emarsys** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emarsys": {
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
