# Legito MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/legito)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate document lifecycle management via Legito — manage template suites, document records, and user permissions directly from any AI agent.

## Description
Connect your **Legito** workspace to any AI agent to streamline your legal and document automation workflows through natural conversation.

### What you can do

- **Document Management** — List document records, retrieve specific version data, and track document shares across your organization.
- **Template Control** — Access and list available template suites and categories to quickly identify the right starting point for new contracts.
- **User & Group Administration** — Manage user groups, list active users, and inspect detailed permissions to ensure secure access control.
- **Global Configuration** — Query workspace info, supported currencies, timezones, and country-specific legal settings.
- **Instant Downloads** — Generate and download document versions in formats like PDF or DOCX directly through your agent.

### How it works

1. Subscribe to this server
2. Enter your Legito Workspace URL, API Key, and Private Key
3. Start managing your document automation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Teams** — instantly find document records and check sharing statuses without leaving your research flow
- **Operations Managers** — automate the retrieval of template suites and manage user group access efficiently
- **HR & Admin** — quickly download generated document versions and verify user permissions during onboarding


## Available Tools (31)
- **add_user_to_group**: Add a user to a user group
- **list_advanced_styles**: List advanced styles
- **list_categories**: List categories (groups)
- **list_countries**: List countries (laws)
- **create_document_version_data**: Create document version data from a template suite
- **create_user_group**: Create a new user group
- **create_user**: Create a new user
- **list_currencies**: List supported currencies
- **delete_document_record**: Delete a document record
- **delete_user_group**: Delete a user group
- **delete_user**: Delete a user
- **list_document_records**: List document records
- **get_document_version_data**: Get data for a specific document version
- **download_document_version**: Download a document version
- **get_info**: Get workspace info
- **remove_share_from_user_group**: Remove a document share from a user group
- **remove_share_from_user**: Remove a document share from a user
- **remove_user_from_group**: Remove a user from a user group
- **share_with_user_group**: Share a document with a user group
- **share_with_user**: Share a document with a user
- **get_shares**: Get shares for a document
- **list_template_suites**: List Legito template suites
- **list_timezones**: List timezones
- **update_document_record**: Update a document record
- **update_document_version_data**: Update document version data
- **update_user_group**: Update a user group
- **update_user_permissions**: Update permissions for a user
- **update_user**: Update a user
- **list_user_groups**: List user groups (departments)
- **get_user_permissions**: Get permissions for a user
- **list_users**: List users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Legito** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all document records currently in the workspace."

**🤖 AI Agent:**
> I've retrieved the document records. You have 12 active records, including 'Service Agreement 2024' (Code: SA-99) and 'Employment Contract - John Doe' (Code: EC-102). Would you like details on a specific one?

---

**👤 You:**
> "Get the data for document version with code 'DOC-5543'."

**🤖 AI Agent:**
> Fetching data for 'DOC-5543'... I've found the version data. It includes 15 metadata fields and was last modified on October 12th. Would you like me to summarize the content or download it?

---

**👤 You:**
> "Download the document 'SA-99' as a docx file."

**🤖 AI Agent:**
> Processing download for 'SA-99' in docx format... Done! You can access the document via this generated link: [Download SA-99.docx].


## ❓ FAQ

**Q: Can I download a specific document version in PDF format?**
Yes! Use the `download_document_version` tool by providing the document code and specifying 'pdf' as the format. Your agent will retrieve the download link or data immediately.

**Q: How do I see all available template suites in my workspace?**
Simply ask the agent to run the `list_template_suites` action. It will return a complete list of all template suites configured in your Legito environment.

**Q: Is it possible to check what permissions a specific user has?**
Yes. By using the `get_user_permissions` tool with a user's identifier, the agent can retrieve the exact permission set assigned to that user in the workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/legito](https://vinkius.com/mcp/legito)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Legito** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `legito` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Legito** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "legito": {
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
