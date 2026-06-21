# NeonCRM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/neoncrm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage non-profit operations via NeonCRM — track donations, memberships, and events directly from your AI agent.

## Description
Connect your **NeonCRM** account to your AI agent and take full control of your non-profit organization's constituent data and fundraising activities through natural conversation.

### What you can do

- **Constituent Management** — List all accounts and contacts to get detailed profiles and historical activity.
- **Donation Tracking** — Access a history of all financial contributions and retrieve metadata for specific donations.
- **Membership Oversight** — Monitor active and historical membership records for your supporters.
- **Event Management** — View all organization events (fundraisers, galas) and registration details.
- **Grant Tracking** — List and inspect grant applications and awards managed within the CRM.
- **Custom Data Access** — Retrieve all standard and custom data fields defined for your CRM profiles.

### How it works

1. Subscribe to this server
2. Enter your NeonCRM Organization ID and API Key
3. Start managing your organization from Claude, Cursor, or any MCP client

### Who is this for?

- **Non-Profit Directors** — quickly check fundraising progress or event details without opening the CRM.
- **Development Teams** — verify donor information and membership statuses during outreach.
- **Operations Managers** — automate the retrieval of grant and constituent lists for reporting.


## Available Tools (10)
- **get_account**: Get specific account details
- **get_donation**: Get donation details
- **get_crm_event**: Get specific event details
- **list_accounts**: List NeonCRM accounts
- **list_contacts**: List CRM contacts
- **list_custom_fields**: List CRM custom fields
- **list_donations**: List all donations
- **list_crm_events**: ) created in NeonCRM.

List CRM events
- **list_grants**: List grant records
- **list_memberships**: List account memberships


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NeonCRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all donations received this year."

**🤖 AI Agent:**
> I've retrieved the donation history for this year. You have 45 contributions totaling $12,450.00. The largest single donation was $1,500.00 from 'Global Impact Foundation'. Would you like the details for that specific donation?

---

**👤 You:**
> "Show me the details for account ID 987."

**🤖 AI Agent:**
> Inspecting account 987... This belongs to 'Jane Smith'. She is a 'Gold Member', has been a constituent since 2018, and has a total lifetime giving of $5,600.00. Shall I list her recent event registrations?

---

**👤 You:**
> "List all upcoming CRM events."

**🤖 AI Agent:**
> Retrieving events... You have 3 upcoming events: 'Annual Spring Gala' (Scheduled: May 15th), 'Community Fun Run' (Scheduled: June 2nd), and 'Quarterly Board Meeting'. Would you like to see the registration list for the Spring Gala?


## ❓ FAQ

**Q: How do I find my NeonCRM Organization ID?**
Your Organization ID (Org ID) is found in your NeonCRM instance URL: https://[OrgID].neoncrm.com.

**Q: Where do I generate an API Key?**
In your NeonCRM dashboard, navigate to Settings > Global Settings > API Settings to find or create your API keys.

**Q: Can I see custom field data?**
Yes! The `get_account` and `get_donation` tools will return custom field values if they are populated, and you can list all available fields using `list_custom_fields`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/neoncrm](https://vinkius.com/mcp/neoncrm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NeonCRM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `neoncrm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NeonCRM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "neoncrm": {
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
