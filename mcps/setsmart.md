# SetSmart MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/setsmart)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Analyze hotel market performance with benchmarking data that compares your property against competitors and market trends.

## Description
Connect your **SetSmart** account to any AI agent and take full control of your multi-channel customer engagement and contact orchestration through natural conversation. SetSmart provides a robust platform for managing business communications via WhatsApp and SMS, and this integration allows you to retrieve contact metadata, send automated messages, and manage tags directly from your chat interface.

### What you can do

- **Contact & Lead Orchestration** — List all managed contacts and retrieve detailed profile metadata, including creating and updating records programmatically.
- **Multi-Channel Messaging** — Send instant WhatsApp and SMS messages to individual customers directly from the AI interface to streamline your outreach.
- **Tag & Segment Control** — List and manage tags to keep your audience segments organized and ensure your communication is properly targeted.
- **Webhook & Automation Oversight** — Access and monitor system webhooks to ensure your conversational data is always synchronized with your business stack.
- **Operational Monitoring** — Track contact activity and manage message logs via natural language commands to ensure reliable customer interactions.

### How it works

1. Subscribe to this server
2. Enter your SetSmart API Key from your dashboard settings
3. Start managing your multi-channel communications from Claude, Cursor, or any MCP-compatible client

No more wrestling with multiple messaging tabs to reach your customers. Your AI acts as a dedicated engagement manager or sales assistant.

### Who is this for?

- **Marketing Managers** — quickly send personalized WhatsApp outreach and monitor contact tags without switching apps.
- **Sales Teams** — automate the management of lead records and track messaging history via natural conversation.
- **Operations Teams** — streamline the retrieval of contact metadata and monitor communication webhooks directly within the chat.


## Available Tools (10)
- **add_tag_to_contact**: Add a tag to a contact
- **create_contact**: Create a new contact
- **delete_contact**: Delete a contact
- **get_contact**: Get contact details by ID
- **list_contacts**: List all contacts
- **list_tags**: List all tags
- **list_webhooks**: List all webhooks
- **send_sms_message**: Send an SMS message
- **send_whatsapp_message**: Send a WhatsApp message
- **update_contact**: Update an existing contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SetSmart** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all contacts tagged as 'High Priority' in SetSmart."

**🤖 AI Agent:**
> I've retrieved your contacts. You have 12 active leads tagged as 'High Priority', including 'Alice Brown' and 'Acme Global'. Would you like to send them a WhatsApp message?

---

**👤 You:**
> "Send a WhatsApp message to +1234567890 saying 'Hello, your appointment is confirmed'."

**🤖 AI Agent:**
> Processing message... The WhatsApp message has been successfully sent to +1234567890. Should I log this activity in the contact's history?

---

**👤 You:**
> "Get the complete details for contact ID 98765."

**🤖 AI Agent:**
> Fetching contact profile... Contact 98765 ('Robert Smith') has email 'robert@example.com' and is tagged with 'Enterprise' and 'New Lead'. Would you like to see their recent message history?


## ❓ FAQ

**Q: Can my AI automatically send a WhatsApp message to a contact by providing their phone number and the text?**
Yes! Use the `send_whatsapp_message` tool. Provide the destination phone number and the content, and your agent will deliver it instantly.

**Q: How do I add a specific tag to a lead for better segmentation?**
Simply ask the agent to run the `add_tag_to_contact` action. You will need the Contact ID and the Tag ID to associate them correctly.

**Q: How do I find my SetSmart API Key?**
Log in to your SetSmart dashboard, navigate to **Settings** > **API**, and you will find your unique secret API Key there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/setsmart](https://vinkius.com/mcp/setsmart)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SetSmart** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `setsmart` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SetSmart** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "setsmart": {
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
