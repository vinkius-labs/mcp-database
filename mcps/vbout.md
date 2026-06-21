# VBOUT MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vbout)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Run marketing campaigns with email automation, social media management, and landing pages in one affordable platform.

## Description
Connect your **VBOUT** marketing automation account to any AI agent and simplify how you manage your lead lifecycle, multi-channel campaigns, and social presence through natural conversation.

### What you can do

- **Lead Management** — List and search contacts, and add new leads to specific email marketing lists instantly.
- **Automation Control** — Query and trigger marketing automation workflows for specific contacts to scale your engagement.
- **Campaign Monitoring** — List active and past marketing campaigns to track your commercial efforts.
- **Social Scheduling** — Create and publish social media posts directly from your workspace via AI commands.
- **E-commerce Sync** — Log customer orders into VBOUT to power lifecycle marketing and personalized segments.

### How it works

1. Subscribe to this server
2. Enter your VBOUT API Key (found in your account settings under API)
3. Start managing your marketing engine from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Managers** — quickly check campaign statuses and publish social updates via simple AI queries.
- **Sales Teams** — add new leads to nurture workflows and retrieve contact details without leaving the CRM or workspace.
- **E-commerce Owners** — sync order data and monitor customer engagement levels directly from the AI assistant.


## Available Tools
- **add_contact**: Requires email and list_id.

Add a contact to a list
- **add_ecommerce_order**: Add an e-commerce order
- **get_contact**: Get contact details
- **list_campaigns**: List marketing campaigns
- **list_email_lists**: List VBOUT email marketing lists
- **list_workflows**: List automation workflows
- **search_contacts**: Search for contacts
- **create_social_post**: Create a social media post
- **trigger_workflow**: Trigger a workflow for a contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VBOUT** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my email marketing lists in VBOUT."

**🤖 AI Agent:**
> I've retrieved your lists. You have 4 active directories: 'Main Newsletter', 'E-book Downloads', 'Webinar Leads', and 'Past Customers'. Which one would you like to add a contact to?

---

**👤 You:**
> "Add 'John Doe' (john@example.com) to the 'Webinar Leads' list."

**🤖 AI Agent:**
> Success! John Doe has been added to the 'Webinar Leads' list (ID: 10293). Shall I trigger the 'Welcome' workflow for him as well?

---

**👤 You:**
> "Post this to my social media: 'Join our upcoming MCP webinar! https://vinkius.com/live'"

**🤖 AI Agent:**
> Social post scheduled! I've sent your content to VBOUT for publishing on your connected channels. The post includes the link to the webinar registration.


## ❓ FAQ

**Q: Can I search for a specific contact using a keyword?**
Yes! Use the `search_contacts` tool and provide your keyword. The agent will return matching contacts from your VBOUT database.

**Q: How do I trigger an automation for a new lead?**
Use the `trigger_workflow` action. You'll need the Workflow ID and the contact's email address to start the automation manually via AI.

**Q: Is it possible to post to my social channels directly?**
Absolutely. Use the `create_social_post` tool, provide your content and an optional link. VBOUT will handle the publishing to your connected profiles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vbout](https://vinkius.com/mcp/vbout)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VBOUT** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `vbout` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VBOUT** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vbout": {
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
