# Adversus MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adversus)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage outbound sales calls, track lead pipelines, and boost call center productivity with intelligent dialing automation.

## Description
Connect your **Adversus** account to any AI agent and take full control of your outbound sales operations, telemarketing, and CRM orchestration through natural conversation.

### What you can do

- **Campaign Orchestration** — List all telemarketing and outreach campaigns programmatically, retrieving detailed status, high-fidelity metadata, and performance metrics in real-time
- **Lead Execution Intelligence** — Programmatically add new contacts and leads to specific campaigns to coordinate your automated dialer and outreach strategy
- **Contact Database Management** — Access complete directories of leads and contacts assigned to campaigns, retrieving high-fidelity profile metadata and relationship history
- **Project & Team Visibility** — Access configured CRM projects and associated campaigns to maintain a perfectly coordinated sales pipeline
- **Operational Monitoring** — Access high-fidelity metadata for account agents and verify API connectivity directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Adversus dashboard (Account Settings > API)
3. Start orchestrating your outbound sales pipeline from Claude, Cursor, or any MCP client

No more manual toggling between dialer tabs or digging through complex lead tables. Your AI acts as your dedicated sales operations coordinator and lead architect.

### Who is this for?

- **Sales Operations Leads** — instantly retrieve campaign performance recaps and manage lead distribution using natural language commands
- **Telemarketing Managers** — coordinate agent assignments and monitor campaign health without leaving your workspace
- **Business Developers** — automate the ingestion of new leads into specialized outreach campaigns through simple AI queries


## Available Tools (7)
- **add_contact_to_campaign**: Add a new contact to a campaign
- **get_campaign_details**: Get details for a specific campaign
- **list_campaigns**: List Adversus campaigns
- **list_campaign_contacts**: List contacts in a campaign
- **list_active_leads**: List global leads
- **list_crm_projects**: List projects
- **list_account_users**: List team users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adversus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active campaigns and their performance in Adversus."

**🤖 AI Agent:**
> I've retrieved your campaigns. You currently have 3 active outreach campaigns, including 'Q2 Renewals' and 'New Business'. One campaign shows a high answer rate. Would you like the detailed high-fidelity metadata for it?

---

**👤 You:**
> "Add 'John Doe' (+15550123) to the 'New Business' campaign (ID: 'camp_456')."

**🤖 AI Agent:**
> Contact orchestrated! I've successfully registered John Doe in the 'New Business' campaign. He is now in the dialer queue and ready for automated outreach. Need help checking his profile history?

---

**👤 You:**
> "Show the last 5 leads captured across all my campaigns."

**🤖 AI Agent:**
> Accessing global leads... I found 5 recent contacts, including @user1 and @user2. All were successfully assigned to their respective high-fidelity sequences. Shall I retrieve the detailed CRM metadata for the most recent lead?


## ❓ FAQ

**Q: How do I find my Adversus API Key?**
Log in to your account, navigate to **Account Settings** > **API**, and generate or copy your unique API Key.

**Q: Can I add a contact to a specific campaign via AI?**
Yes! The `add_contact_to_campaign` tool allows your agent to register new leads programmatically by providing the campaign ID and phone number.

**Q: How do I check my global leads?**
Use the `list_active_leads` tool to retrieve a comprehensive directory of all contacts across your entire Adversus account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adversus](https://vinkius.com/mcp/adversus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Adversus** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `adversus` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Adversus** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adversus": {
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
