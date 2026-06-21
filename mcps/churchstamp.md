# ChurchStamp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/churchstamp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage church operations with member directories, event planning, volunteer coordination, and donation tracking for ministries.

## Description
Connect your **ChurchStamp** account to any AI agent and take full control of your physical direct mail orchestration and automated postcard outreach through natural conversation.

### What you can do

- **Postal Outreach Orchestration** — Programmatically send personalized postcards and letters to recipients, retrieving detailed technical status in real-time
- **Campaign Intelligence** — Programmatically retrieve lists of active direct mail campaigns and access complete performance metadata for your mobile outreach
- **Design Portfolio Architecture** — Access your complete directory of mail designs and templates to maintain a perfectly coordinated brand presence
- **Delivery Monitoring** — Access real-time status updates for mail pieces and track campaign progress directly through your agent for instant operational reporting
- **Infrastructure Verification** — Verify account-level API connectivity and monitor mailing volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **Access Token** from your ChurchStamp dashboard (Settings > Security)
3. Start orchestrating your physical outreach from Claude, Cursor, or any MCP client

No more manual uploading of recipient CSVs or guessing mail delivery dates. Your AI acts as your dedicated mail coordinator and direct marketing architect.

### Who is this for?

- **Church Administrators** — instantly trigger welcome postcards and monitor outreach campaigns using natural language commands
- **Marketing Operations** — verify mail design metadata and track campaign results without leaving your creative workspace
- **Outreach Coordinators** — automate the management of recipient lists and mail piece assignments through simple AI queries


## Available Tools
- **check_churchstamp_status**: Verify ChurchStamp API connectivity
- **create_campaign**: Optionally assign a design template.

Create a mail campaign
- **create_contact**: Add a contact
- **get_campaign**: Get campaign details
- **get_design**: Get design details
- **get_user_details**: Get your account
- **list_campaigns**: List all mail campaigns
- **list_contacts**: List all contacts
- **list_designs**: List all postcard designs
- **send_mail**: Send a postcard


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ChurchStamp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a 'Welcome Postcard' (Design ID: ds_123) to 'John Doe' at '123 Main St, London, SW1A 1AA'."

**🤖 AI Agent:**
> Mail orchestrated! I've successfully triggered the sending of your 'Welcome Postcard' to John Doe. The transmission ID is mail_987. Shall I notify you once the delivery status is confirmed?

---

**👤 You:**
> "List all active direct mail campaigns in my ChurchStamp account."

**🤖 AI Agent:**
> Campaign directory orchestrated! You currently have 5 active portfolios, including 'Christmas Outreach' and 'New Member Welcome'. Would you like the detailed performance metadata for any of them?

---

**👤 You:**
> "Show my available mail designs and templates."

**🤖 AI Agent:**
> Design architecture orchestrated! I've identified 3 mail designs, including 'Modern Postcard' and 'Standard Letter'. I've retrieved the technical metadata for your next campaign. Need help selecting a design for a new recipient?


## ❓ FAQ

**Q: How do I find my ChurchStamp Access Token?**
Log in to your account, navigate to **Settings** > **Security**, and copy your unique Access Token from the API section.

**Q: Can I send personalized postcards via AI?**
Yes! The `send_churchstamp_mail` tool allows your agent to trigger physical mailings by providing recipient metadata and design IDs.

**Q: How do I list my mail designs?**
Use the `list_designs` tool to retrieve your complete directory along with the unique identifiers for all managed templates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/churchstamp](https://vinkius.com/mcp/churchstamp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ChurchStamp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `churchstamp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ChurchStamp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "churchstamp": {
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
