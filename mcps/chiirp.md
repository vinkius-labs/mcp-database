# Chiirp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chiirp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Engage leads and customers through automated text, email, and voicemail campaigns that nurture relationships at scale.

## Description
Connect your **Chiirp** account to any AI agent and manage your lead automation CRM through natural conversation.

### What you can do

- **Contacts** — Create, search, update, and list contacts with full CRM metadata.
- **Tags** — Apply and remove tags to segment contacts and trigger automations.
- **Campaigns** — View active SMS and drip campaigns with engagement data.
- **Sequences** — Monitor automation sequences and drip workflows.
- **Profile** — Access your account profile and verify API connectivity.

### How it works

1. Subscribe to this server
2. Enter your Chiirp API token from your dashboard
3. Start managing leads from Claude, Cursor, or any MCP client

### Who is this for?

- **Home Service Businesses** — manage leads and automate follow-up sequences.
- **Sales Teams** — tag and segment contacts for targeted outreach.
- **Marketing Managers** — monitor campaign performance and drip sequence engagement.


## Available Tools
- **apply_tag**: Useful for segmentation and triggering automations.

Apply a tag to a contact
- **check_chiirp_status**: Verify Chiirp API connectivity
- **create_contact**: Phone number is required as the unique identifier.

Create a new contact
- **get_contact**: Get details of a specific contact
- **get_profile**: Get your Chiirp account profile
- **list_campaigns**: List all campaigns
- **list_contacts**: List all contacts in your Chiirp account
- **list_sequences**: List all automation sequences
- **list_tags**: List all available tags
- **remove_tag**: Remove a tag from a contact
- **search_contacts**: Search contacts by phone number
- **update_contact**: Only provided fields are changed.

Update an existing contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chiirp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my contacts in Chiirp."

**🤖 AI Agent:**
> You have 247 contacts. The most recent are: John Smith (+1-555-0101, tagged 'hot-lead'), Maria Garcia (+1-555-0202, tagged 'hvac-customer'), and David Lee (+1-555-0303).

---

**👤 You:**
> "Apply the 'hot-lead' tag to the contact with phone +1-555-0303."

**🤖 AI Agent:**
> Done! The 'hot-lead' tag has been applied to David Lee (+1-555-0303). This triggered the 'Hot Lead Follow-up' drip sequence automatically.

---

**👤 You:**
> "Create a new contact for +1-555-0404 named Sarah Johnson."

**🤖 AI Agent:**
> New contact created: Sarah Johnson (+1-555-0404). The contact is now in your Chiirp CRM and ready for tagging or campaign enrollment.


## ❓ FAQ

**Q: Can I search for a contact by phone number?**
Yes! Use `search_contacts` with the phone number to find matching contacts in your Chiirp database.

**Q: How do I add a tag to trigger an automation?**
Use `apply_tag` with the contact's phone number and the tag ID. If the tag is linked to an automation sequence in Chiirp, it will trigger automatically.

**Q: Can I view my active campaigns?**
Yes! Use `list_campaigns` to see all SMS and drip campaigns, or `list_sequences` to view automation workflows with their statuses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chiirp](https://vinkius.com/mcp/chiirp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chiirp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `chiirp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chiirp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chiirp": {
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
