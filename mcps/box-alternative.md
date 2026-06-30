# Box MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/box-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Store, share, and collaborate on files securely with enterprise-grade cloud content management and governance controls.

## Description
Connect your **Box** account to any AI agent and take full control of your cloud content management and enterprise collaboration workflows through natural conversation.

### What you can do

- **Folder Orchestration** — Navigate through your entire Box directory structure programmatically, listing folder items and retrieving high-fidelity metadata in real-time
- **File Lifecycle Management** — Access detailed information about individual files, including version history, size, and high-fidelity descriptions directly through your agent
- **Collaboration Intelligence** — Programmatically manage folder collaborations by inviting team members with specific roles (editor, viewer) to ensure perfectly coordinated access
- **Search & Discovery** — Use semantic keywords to search for specific files and folders across your entire Box account to maintain a perfectly coordinated digital library
- **User Visibility** — Retrieve complete profile information for the authenticated user and manage account-level metadata for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Developer Token** (for testing) or **Access Token** (OAuth) from the Box Developer Console
3. Start managing your enterprise content from Claude, Cursor, or any MCP client

No more manual searching through browser tabs to find specific documents or check permissions. Your AI acts as your dedicated cloud content manager and digital librarian.

### Who is this for?

- **Project Managers** — instantly retrieve project files and manage team access using natural language commands
- **Knowledge Workers** — verify document versions and search for internal resources without leaving your workspace
- **IT & Admin Leads** — automate organizational file auditing and collaboration oversight through simple AI queries


## Available Tools (10)
- **create_collaboration**: Requires the folder ID, the user's email (login), and an assigned role (e.g., "editor", "viewer", "previewer").

Share a folder with a collaborator
- **create_folder**: Use parent ID "0" for the root folder.

Create a new folder in Box
- **delete_file**: Delete a file from Box
- **delete_folder**: If the folder is not empty, you must set the recursive flag to true to delete all its contents.

Delete a folder from Box
- **get_file_info**: Includes size, SHA1 hash, version information, and parent folder details.

Get details and metadata for a file
- **get_folder_info**: Includes information about the parent folder, creator, and modified dates.

Get details and metadata for a folder
- **list_folder_items**: Note: Use ID "0" for the root folder.

List all items within a folder
- **search_content**: Useful for discovering items when the IDs are unknown.

Search for files and folders
- **update_file**: Can be used to rename the file or update its description.

Update file attributes and metadata
- **get_current_user**: Use this to verify the current identity.

Retrieve current Box user details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Box** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all items in my Box root folder."

**🤖 AI Agent:**
> I've retrieved your root directory. You currently have 5 items, including 'Project Alpha' (Folder ID: 123) and 'Quarterly Reports'. Which one should we explore for details?

---

**👤 You:**
> "Search for files containing 'Invoice' in my Box account."

**🤖 AI Agent:**
> Searching... I found 3 matching files: 'Invoice_April_2026.pdf' (ID: 456), 'Old_Invoice.docx', and 'Pending_Invoice'. Would you like the high-fidelity metadata for the April invoice?

---

**👤 You:**
> "Invite @user1 to folder '123' as an editor."

**🤖 AI Agent:**
> Collaboration created! I've successfully invited @user1 to collaborate on specified folder (ID: 123) with the 'editor' role. They will receive a notification to join. Need help with any other access controls?


## ❓ FAQ

**Q: How do I find my Box Access Token?**
Log in to the [**Box Developer Console**](https://app.box.com/developers/console), select your app, and generate a Developer Token or use the OAuth settings to obtain an Access Token.

**Q: Can I search for content via AI?**
Yes! The `search_content` tool allows your agent to find files and folders across your entire account matching specific keywords.

**Q: How do I share a folder programmatically?**
Use the `create_collaboration` tool and provide the folder ID, the recipient's email (login), and their assigned role (e.g., 'editor', 'viewer').


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/box-alternative](https://vinkius.com/mcp/box-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Box** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `box-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Box** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "box-alternative": {
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
