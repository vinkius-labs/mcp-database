# DottedSign MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dottedsign-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate e-signature workflows via DottedSign — create signing tasks, manage templates, and track document status directly from any AI agent.

## Description
Connect your **DottedSign** account to any AI agent to streamline your document signing processes through natural conversation.

### What you can do

- **Task Management** — Create signing tasks from files or templates, update signers, and track progress in real-time.
- **Template Utilization** — List and retrieve available templates to quickly generate standardized signing requests.
- **Lifecycle Control** — Void, archive, or discard tasks as needed, and restore documents from the trash when necessary.
- **File Missions** — Handle complex multi-file uploads and missions before initiating formal signing tasks.
- **Status Tracking** — Query specific task details to see who has signed and who is still pending.

### How it works

1. Subscribe to this server
2. Enter your DottedSign Personal Access Token
3. Start managing your legal and business documents from Claude, Cursor, or any MCP client

No more manual tracking of pending contracts. Your AI acts as a digital legal assistant, ensuring no signature is missed.

### Who is this for?

- **Legal & Compliance Teams** — quickly verify the status of multiple contracts and manage document archives.
- **Sales Operations** — automate the creation of signing tasks from templates as soon as a deal closes.
- **HR Departments** — streamline onboarding by sending and tracking employee handbooks and NDAs.


## Available Tools (25)
- **archive_task**: Archive a DottedSign task
- **create_file_mission**: Create a file mission
- **create_public_form**: Create a public form
- **create_task**: Create a new DottedSign task
- **delete_public_form**: Delete a public form
- **discard_task**: Discard a DottedSign task
- **get_file_mission_download_link**: Get a download link for mission files
- **get_file_mission**: Get file mission details
- **get_groups**: Get group info
- **get_me**: Get current member info
- **get_public_form**: Get details of a specific public form
- **get_task**: Get detailed information about a specific task
- **get_template**: Get details of a specific template
- **list_public_forms**: Get a list of active public forms
- **list_tasks**: Get a list of DottedSign tasks
- **list_templates**: Get a list of available templates
- **quick_create_task**: Quick create a DottedSign task
- **renew_file_mission**: Renew a file mission
- **restore_task**: Restore a DottedSign task
- **unarchive_task**: Unarchive a DottedSign task
- **update_groups**: Update group info
- **update_me**: Update current member info
- **update_public_form**: Update a public form
- **update_task**: Update a DottedSign task
- **void_task**: Void a DottedSign task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DottedSign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my pending signing tasks on DottedSign."

**🤖 AI Agent:**
> I've retrieved your tasks. You have 3 tasks waiting for signatures, including 'Service Agreement' (ID: ds_882) and 'NDA - New Hire' (ID: ds_901). Would you like details on any of these?

---

**👤 You:**
> "Create a quick signing task using template ID 'temp_554'."

**🤖 AI Agent:**
> Task created successfully using the template! The new task ID is 'ds_1029'. I have sent the document to the default signers defined in the template.

---

**👤 You:**
> "Show me the full details for task ds_882."

**🤖 AI Agent:**
> Inspecting task ds_882... The document 'Service Agreement' is currently in 'waiting' status. Signer 'Alice Smith' has viewed it but not yet signed, while 'Bob Jones' has not opened it yet.


## ❓ FAQ

**Q: Can I see exactly who has signed a document using the task ID?**
Yes. Use the `get_task` tool with the specific Task ID. The agent will return the full status, including signer information and current progress of the document.

**Q: How do I quickly send a document using a predefined template?**
First, use `list_templates` to find the correct Template ID, then use the `quick_create_task` tool to initiate the signing process using the template's default settings.

**Q: Is it possible to recover a task that was accidentally moved to the trash?**
Absolutely. You can use the `restore_task` tool with the Task ID to move any discarded document back to your main task list.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dottedsign-alternative](https://vinkius.com/mcp/dottedsign-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DottedSign** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dottedsign-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DottedSign** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dottedsign-alternative": {
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
