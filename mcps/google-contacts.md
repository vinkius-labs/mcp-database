# Google Contacts MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-contacts)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Google Contacts network seamlessly — list, search, create, and organize contacts and groups directly from any AI agent.

## Description
Connect your **Google Contacts** directory to any AI agent and take full control of your address book and connections through natural conversation.

### What you can do

- **Contact Management** — Query, lookup, create, and update contact profiles effortlessly
- **Group Synchronization** — List organizational groups and filter contacts by labels directly from the cloud
- **Deep Search** — Run intelligent lookups by names, emails, and attributes across your entire address book

### How it works

1. Subscribe to this server
2. Authenticate securely with your Google Workspace account
3. Start managing directories from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales & SDR Teams** — instantly retrieve prospect details or update contact cards right from conversational interfaces
- **Executive Assistants** — quickly build groupings, organize network contacts, and manage connections
- **Developers** — fetch precise contact information straight from the IDE without opening external windows


## Available Tools (9)
- **create_contact_group**: 
- **create_contact**: Creates a new contact (connection)
- **delete_contact**: Deletes a contact
- **get_contact_group**: 
- **get_contact**: Gets the full details of a specific contact
- **list_contact_groups**: Lists the user's contact groups (or labels)
- **list_contacts**: Lists the user's connections (contacts)
- **search_contacts**: Searches the user's contacts by a query string
- **update_contact**: Must provide an etag obtained from get_contact.

Updates an existing contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Contacts** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my contacts for John Doe and give me his phone number."

**🤖 AI Agent:**
> Scanning directory... I reached John Doe. His primary mobile number is registered as +1 (555) 123-4567 and his core email is john.doe@example.com.

---

**👤 You:**
> "Create a new contact named Alice Smith with email alice@example.com"

**🤖 AI Agent:**
> Successfully issued creation. The identity 'Alice Smith' has been persisted correctly with ID 'people/c230919321', keeping 'alice@example.com' as her primary routing channel.

---

**👤 You:**
> "List all organizational contact groups available."

**🤖 AI Agent:**
> I've fetched the segments. Found 3 notable groupings mapping connections: 'Starred in Android' (32 users), 'Lead Funnel 2024' (81 prospects), and 'Tech Advisors' (5 users). Would you like to check the Advisors list?


## ❓ FAQ

**Q: Which exact service and endpoints does this utilize?**
This integration leverages the highly structured Google People API. It strictly filters and returns core metadata (emails, names, numbers) avoiding unnecessary heavy payloads.

**Q: Can it automatically assign new prospects into specific mailing groups?**
Certainly. The `create_contact` tool allows passing a specific Group Identifier (which you can discover using `list_contact_groups`). The user will instantly appear in the matching mailing segment.

**Q: What happens if I try to list a corporate directory with thousands of interconnected contacts?**
The integration is protected by aggressive egress control pagination features out-of-the-box. Your AI agent handles paginated loops automatically and queries intelligent searches to restrict context overhead limits naturally.

**Q: Is it possible to manage shared domain profiles or only my personal Gmail connections?**
Assuming you are logged in using a Google Workspace suite, the authorization supports cross-referencing domain contacts. Personal Gmail queries apply strict visibility bounding towards individual connections only.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-contacts](https://vinkius.com/mcp/google-contacts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Contacts** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `google-contacts` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Contacts** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-contacts": {
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
