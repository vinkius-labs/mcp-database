# Transloadit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/transloadit-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Versatile file uploading and processing API.

## Description
The Transloadit MCP server allows your AI agent to orchestrate complex file processing pipelines. Trigger encodings, convert documents, resize images, and monitor assembly statuses right from your conversation.


## Available Tools
- **cancel_assembly**: Stop a currently running assembly
- **create_assembly**: Start a new file processing assembly
- **create_template**: Create a new processing template
- **delete_template**: Permanently remove a template
- **get_assembly**: Retrieve status and results for a specific assembly
- **get_bill**: Retrieve billing information for a specific month
- **get_me**: Check API connectivity and get account context
- **get_template**: Retrieve details for a specific template
- **list_assemblies**: List all file processing assemblies
- **list_templates**: List all reusable processing templates
- **replay_assembly**: Re-run a completed assembly
- **update_template**: Update an existing template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Transloadit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available Transloadit templates."

**🤖 AI Agent:**
> You have 2 templates: 'Video to MP4' (ID: 99a1) and 'Image Resize 500px' (ID: 99a2).

---

**👤 You:**
> "Check the status of Assembly ID 88392."

**🤖 AI Agent:**
> Assembly 88392 is 'COMPLETED'. The processed file is available at the output URL.

---

**👤 You:**
> "Cancel the processing for Assembly ID 99120."

**🤖 AI Agent:**
> Assembly ID 99120 has been successfully canceled and removed from the queue.


## ❓ FAQ

**Q: Can I check the status of a specific file assembly?**
Yes, just provide the Assembly ID to the agent, and it will return the real-time processing status and output URLs.

**Q: Does it support triggering new conversions?**
You can trigger new pipelines if you supply a valid Template ID and the source file URLs.

**Q: How do I list my active templates?**
Ask the AI to 'List all Transloadit templates' and it will retrieve your available processing recipes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/transloadit-alternative](https://vinkius.com/mcp/transloadit-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Transloadit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `transloadit-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Transloadit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "transloadit-alternative": {
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
