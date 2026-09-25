# Reamaze MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reamaze)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate customer support and helpdesk workflows via Reamaze — manage help articles, channels, and contacts directly from any AI agent.

## Description
Connect your **Reamaze** account to any AI agent to streamline your customer support operations and knowledge base management through natural conversation.

### What you can do

- **Knowledge Base Management** — List, retrieve, create, and update help articles to keep your documentation synchronized.
- **Channel Oversight** — Inspect active support channels including email, chat, and social media integrations to understand your support surface.
- **Contact Management** — Search for customer profiles, create new contacts, and update existing user data to maintain a clean CRM.
- **Article Search** — Query your help center using keywords or status filters to find the exact information your customers need.

### How it works

1. Subscribe to this server
2. Enter your Reamaze Brand name, Login Email, and API Token
3. Start managing your support ecosystem from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Leads** — quickly audit help center content and monitor active communication channels.
- **Customer Success Managers** — update contact information and custom data fields without leaving the conversation.
- **Content Strategists** — draft and update help articles directly through AI assistance.


## Available Tools (34)
- **list_articles**: Can be scoped to a topic slug, filtered by status, or searched.

List Help Articles for the Brand
- **list_identities**: Pass the contact’s email address.

Retrieve identities for a contact
- **list_staff**: Retrieve staff users for the Account
- **create_staff**: Pass the complete staff payload containing all required user details.

Create a new staff user
- **delete_contact_note**: Provide both the note ID and the contact identifier.

Delete a contact note
- **get_article**: Provide the exact article slug as input.

Retrieve a specific Help Article
- **get_channel**: Provide the unique slug of the channel.

Retrieve a specific channel
- **get_conversation**: Pass the unique conversation slug.

Retrieve a specific conversation
- **get_response_template**: Use the unique template ID.

Retrieve a specific Response Template
- **list_contact_notes**: Use the contact email or phone number as the identifier.

Retrieve notes for a specific contact
- **list_contacts**: Use the ’q’ parameter to filter results.

List contacts for the Account
- **list_messages**: Set ’include’ to "original_body" to get HTML content.

Retrieve individual messages for all conversations
- **list_satisfaction_ratings**: Retrieve satisfaction survey ratings
- **update_contact_note**: Use the identifier to locate the correct contact.

Update a contact note
- **update_conversation**: Specify the conversation slug and the payload to modify.

Update a conversation
- **create_article**: Ensure the article payload includes a title and body.

Create a new Help Article
- **create_contact**: Provide at least a name or email address.

Create a new contact
- **create_contact_note**: You must specify the contact’s identifier and the note content.

Attach a note to a contact
- **create_conversation**: Supply required customer details and initial message.

Create a new conversation on behalf of a customer
- **create_identity**: Provide the contact’s email address.

Attach an identity to a contact
- **create_incident**: Pass the complete incident payload containing all necessary details.

Create a new incident
- **create_message**: Provide the conversation slug and message body.

Create a new message under a specific conversation
- **create_response_template**: Supply the required template payload.

Create a new Response Template
- **get_incident**: Pass the unique identifier of the incident you wish to retrieve.

Retrieve a specific incident
- **get_report**: Retrieve a specific report
- **list_channels**: List channels for the Brand
- **list_conversations**: Filter results using tags, categories, or origin.

List conversations for the Brand
- **list_incidents**: Retrieve incidents for the Brand
- **list_response_templates**: Retrieve Response Templates for the Brand
- **list_systems**: The function executes asynchronously.

Retrieve systems for the Brand
- **update_article**: You must provide both the article slug and the updated payload.

Update a specific Help Article
- **update_contact**: Specify the contact identifier and the fields to modify.

Update a specific contact
- **update_incident**: Specify the incident identifier and the payload containing changes.

Update a specific incident
- **update_response_template**: Provide the template slug and the full payload to modify the content.

Update a specific response template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reamaze** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for help articles related to 'refund policy' and list them."

**🤖 AI Agent:**
> I found 2 articles matching 'refund policy': 'Standard Refund Procedure' (slug: standard-refund) and 'International Returns' (slug: international-returns). Would you like to see the content of one of them?

---

**👤 You:**
> "Create a new contact for John Doe with email john@example.com."

**🤖 AI Agent:**
> I have successfully created the contact for John Doe (john@example.com). The profile is now active in your Reamaze account.

---

**👤 You:**
> "List all active email channels for our brand."

**🤖 AI Agent:**
> I've retrieved your email channels. You have 2 active: 'Support Main' (support@brand.com) and 'Sales Inquiry' (sales@brand.com).


## ❓ FAQ

**Q: Can I search for specific customers using their email address?**
Yes. You can use the `list_contacts` tool with the `q` parameter to search for contacts by name or email address across your entire account.

**Q: Is it possible to update an existing help article's content?**
Absolutely. Use the `update_article` tool by providing the article's slug and the updated JSON payload containing the new title, body, or status.

**Q: How can I see which communication channels are connected to my brand?**
You can use the `list_channels` tool to retrieve all active channels. You can also filter them by type, such as 'email', 'chat', or 'facebook'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reamaze](https://vinkius.com/en/ai-agent-connect/reamaze)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reamaze** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reamaze` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reamaze** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reamaze": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
