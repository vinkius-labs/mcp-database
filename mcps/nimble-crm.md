# Nimble CRM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nimble-crm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage relationships and deals via Nimble CRM — track contacts, deals, and activities directly from your AI agent.

## Description
Connect your **Nimble CRM** account to your AI agent and streamline your relationship management and sales pipelines through natural conversation.

### What you can do

- **Contact Management** — List all people and companies and search for specific profiles based on keywords, emails, or notes.
- **Sales Pipelines** — Access all deals and opportunities, including their current stage, value, and expected close dates.
- **Activity Tracking** — Monitor your tasks, calendar events, and calls to stay on top of your schedule.
- **Relationship Intelligence** — Fetch complete metadata and social profiles for specific contacts to better prepare for meetings.
- **Note Taking** — Attach new notes or log entries directly to contact profiles within your chat.
- **Organization Oversight** — View all defined deal pipelines and retrieve your own user metadata.

### How it works

1. Subscribe to this server
2. Enter your Nimble CRM API Key
3. Start managing your relationships from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales Professionals** — quickly look up a contact's details or add a follow-up note after a call without opening the CRM.
- **Account Managers** — monitor deal progress and activity history directly from your workspace.
- **Business Owners** — automate the retrieval of deal lists and pipeline statuses for daily standups.


## Available Tools
- **add_note_to_contact**: Add a note to a contact
- **get_activity**: Get specific activity details
- **get_contact**: Get specific contact details
- **get_deal**: Get specific deal info
- **get_me**: Get current user info
- **list_activities**: List tasks and events
- **list_contacts**: List Nimble contacts
- **list_deals**: List Nimble deals
- **list_pipelines**: List deal pipelines
- **search_contacts**: Search for contacts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nimble CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all people and companies in my Nimble CRM."

**🤖 AI Agent:**
> Retrieving contacts... I found several contacts including 'John Smith' (Acme Corp), 'Sarah Jenkins' (Global Tech), and 'Innovate Solutions'. Would you like the details for John Smith?

---

**👤 You:**
> "Search for a contact with the email 'ryan@example.com'."

**🤖 AI Agent:**
> Searching... I've found a profile for 'Ryan Howard'. He is a 'Director' at 'Dunder Mifflin' and has 3 active tags: 'High Priority', 'Lead', and 'Q4-Focus'. Shall I retrieve his recent activity history?

---

**👤 You:**
> "What are my current active deals?"

**🤖 AI Agent:**
> Retrieving deals... You have 5 active deals totaling $45,000. Highlights include 'Enterprise Upgrade' ($20K - Negotiation) and 'Consulting Phase 1' ($5K - Qualification). Would you like the full pipeline breakdown?


## ❓ FAQ

**Q: How do I get a Nimble CRM API Key?**
Log in to Nimble, go to Settings > API Keys, and click 'Generate New Token'. This key is used for authentication.

**Q: Can I search for contacts by email?**
Yes! Use the `search_contacts` tool and provide the email address as the keyword. Nimble will return matching profiles.

**Q: How do I see my sales stages?**
Use the `list_pipelines` tool to retrieve all your deal pipelines and the specific stages defined for each one.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nimble-crm](https://vinkius.com/mcp/nimble-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nimble CRM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nimble-crm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nimble CRM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nimble-crm": {
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
