# Close MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/close-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Close more deals with a CRM that puts calling, emailing, and pipeline management in one fast interface built for inside sales.

## Description
Connect your **Close** CRM account to any AI agent and take full control of your sales workflows through natural conversation.

### What you can do

- **Lead Management** — List all leads in your pipeline and retrieve full company profiles with contacts, custom fields, and activity history
- **Lead Creation** — Add new leads directly from conversation, including company name and website URL
- **Opportunity Tracking** — Monitor your active deals with stage, value, and expected close dates
- **Task Management** — Review pending and completed CRM tasks to stay on top of follow-ups
- **User Context** — Retrieve your authenticated user profile to understand your current permissions and role

### How it works

1. Subscribe to this server
2. Enter your Close API Key from Settings > Developer > API Keys
3. Start managing your sales pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Representatives** — query your pipeline, check lead details, and create new prospects without leaving your AI workspace
- **Sales Managers** — monitor team opportunities and task completion rates through conversational analytics
- **Revenue Operations** — automate lead creation workflows and pipeline visibility across the organization


## Available Tools
- **create_lead**: Create a new lead
- **get_lead_details**: Get details of a specific lead
- **get_current_user**: Get information about the authenticated API user
- **list_leads**: List all leads in Close CRM
- **list_opportunities**: List sales opportunities
- **list_crm_tasks**: List CRM tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Close** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my leads in Close and highlight the ones added this week."

**🤖 AI Agent:**
> I retrieved 47 leads from your Close account. 5 were added this week: 'Acme Corp' (lead_8291), 'TechFlow Inc' (lead_8294), 'DataBridge Solutions' (lead_8297), 'NovaPay' (lead_8301), and 'Quantum Systems' (lead_8305). Would you like to see the full details for any of these?

---

**👤 You:**
> "Create a new lead for the company 'Nordic AI Labs' with their website nordicailabs.com."

**🤖 AI Agent:**
> Done! Lead created successfully. The new Lead ID is lead_8312 for 'Nordic AI Labs' with URL nordicailabs.com. The record is now active in your pipeline. Would you like me to check for existing opportunities or create a follow-up task?

---

**👤 You:**
> "Show my active sales opportunities and any overdue tasks I need to handle."

**🤖 AI Agent:**
> You have 12 active opportunities worth a total of $284,500. The top 3 by value: 'Enterprise Deal - Acme Corp' ($85,000, Negotiation stage), 'DataBridge Annual Contract' ($52,000, Proposal stage), and 'TechFlow Migration' ($41,000, Demo stage). You also have 3 overdue tasks: a call with Acme Corp (2 days late), a proposal follow-up for DataBridge (1 day late), and a meeting note for NovaPay (3 days late).


## ❓ FAQ

**Q: Can I create new leads directly through the AI agent?**
Yes! The `create_lead` tool accepts a company name and an optional website URL. Your agent will create the lead record in Close and return the new Lead ID for immediate reference.

**Q: How does the API authentication work with Close?**
Close uses HTTP Basic Authentication. Your API Key is sent as the username with an empty password. Navigate to Settings > Developer > API Keys in your Close dashboard to generate a new key. The key is encrypted at rest and injected securely at runtime.

**Q: Can I view my sales opportunities and their current stages?**
Yes. The `list_opportunities` tool retrieves all active deals in your pipeline, including stage name, expected value, probability, and projected close date. Combine it with `list_crm_tasks` to check pending follow-ups associated with each opportunity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/close-alternative](https://vinkius.com/mcp/close-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Close** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `close-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Close** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "close-alternative": {
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
