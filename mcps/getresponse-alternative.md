# GetResponse MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/getresponse-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Grow your audience with email marketing, landing pages, webinars, and marketing automation that works together seamlessly.

## Description
Connect your **GetResponse** account to any AI agent and take full control of your email marketing and automation workflows through natural conversation.

### What you can do

- **Audience Orchestration** — List and manage your email subscribers programmatically, including retrieving detailed metadata and performing lookups by email
- **Campaign Management** — Monitor your marketing lists and campaigns and retrieve detailed configuration data to track performance
- **Automation Intelligence** — Access autoresponder sequences and workflow settings to coordinate automated customer journeys
- **Lead Generation** — Monitor published landing pages and manage subscriber registrations directly through your agent to drive growth
- **Custom CRM Fields** — Retrieve and manage custom contact fields to maintain a structured and personalized marketing ecosystem

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your GetResponse account (Tools > Integrations and API > API)
3. Start managing your marketing automation from Claude, Cursor, or any MCP client

No more manual subscriber lookups or complex campaign navigation. Your AI acts as your dedicated marketing operations assistant.

### Who is this for?

- **Digital Marketers** — instantly retrieve campaign details and update subscriber lists using natural language queries
- **E-commerce Owners** — monitor lead generation from landing pages and manage autoresponders without leaving your workspace
- **Customer Success Managers** — verify subscriber data and manage custom fields through automated AI searches


## Available Tools (12)
- **add_new_subscriber**: Register new contact
- **remove_subscriber**: Delete a contact
- **get_api_status**: Check connection
- **get_list_details**: Get campaign info
- **get_contact_details**: Get subscriber info
- **list_active_sequences**: Get autoresponders
- **list_marketing_lists**: List email campaigns
- **list_email_contacts**: List your subscribers
- **list_contact_fields**: Get custom fields
- **list_published_pages**: Get landing pages
- **list_active_webhooks**: Get event configs
- **find_contact_by_email**: Search subscribers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GetResponse** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my marketing campaigns in GetResponse."

**🤖 AI Agent:**
> I've retrieved your marketing lists. You have 3 active campaigns: 'Weekly Newsletter' (ID: abc), 'Product Updates' (ID: def), and 'Lead Magnet' (ID: ghi). Which one would you like to manage?

---

**👤 You:**
> "Add 'john.doe@example.com' to my 'Product Updates' campaign."

**🤖 AI Agent:**
> Done! I've registered John Doe (john.doe@example.com) to the 'Product Updates' campaign (ID: def). They will now receive your scheduled emails for this list.

---

**👤 You:**
> "Find subscriber details for 'sarah@example.com'."

**🤖 AI Agent:**
> I've located Sarah's profile. She joined the 'Weekly Newsletter' on 2024-03-15 and is currently an active subscriber. Would you like to see her custom field values or activity status?


## ❓ FAQ

**Q: How do I find my GetResponse API Key?**
Log in to your account, navigate to **Tools** > **Integrations and API**, and select the **API** tab to generate or copy your key.

**Q: Can I add a contact to a specific list?**
Yes! Use the `add_new_subscriber` tool and provide the `campaignId` of the target list along with the contact's email.

**Q: How do I search for a subscriber by email?**
The `find_contact_by_email` tool allows you to perform a direct lookup to retrieve a specific subscriber's profile and metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/getresponse-alternative](https://vinkius.com/mcp/getresponse-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GetResponse** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `getresponse-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GetResponse** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "getresponse-alternative": {
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
