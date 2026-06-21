# autoRetouch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/autoretouch)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Retouch product photos at scale with AI-powered background removal, color correction, and beauty editing for e-commerce.

## Description
Connect your **autoRetouch** account to any AI agent and take full control of your automated image editing and high-fidelity retouching workflows through natural conversation.

### What you can do

- **Workflow Orchestration** — Execute complex high-fidelity AI workflows for background removal, color correction, and shadow generation programmatically
- **Bulk Processing Intelligence** — Programmatically upload raw images and monitor their processing status in real-time to maintain a perfectly coordinated media pipeline
- **Result Discovery** — Retrieve high-fidelity result URLs for processed images and access detailed metadata for every individual execution
- **Lifecycle Management** — Group multiple executions into tracked batches to oversee your organization's image editing volume efficiently
- **Financial Visibility** — Access your organization's wallet balance and profile metadata directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** and **Organization ID** from your autoRetouch dashboard (API settings)
3. Start localizing and retouching your media assets from Claude, Cursor, or any MCP client

No more manual dragging into web tools for repeatable editing tasks. Your AI acts as your dedicated digital imaging engineer and workflow coordinator.

### Who is this for?

- **E-commerce Merchants** — instantly process high-volume product photos for catalog updates using natural language commands
- **Marketing Agencies** — automate the removal of backgrounds and color balancing without leaving your creative workspace
- **Photographers** — orchestrate complex retouching sequences across large batches through simple AI queries


## Available Tools (11)
- **create_execution**: Returns the execution ID.

Start an image processing execution
- **get_batch**: Get details of a specific batch
- **get_execution**: Get details of a specific execution
- **get_image**: Get details of a specific image
- **get_organization**: Get organization details
- **get_wallet_balance**: Get account wallet balance
- **get_workflow**: Get details of a specific workflow
- **list_batches**: List all batches
- **list_executions**: List recent executions
- **list_images**: List uploaded images
- **list_workflows**: List all image processing workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **autoRetouch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active image processing workflows in my organization."

**🤖 AI Agent:**
> I've retrieved your workflows. You currently have 3 active AI pipelines: 'Ghost Mannequin' (ID: wf_123), 'Shadow Gen', and 'Bulk Background Remove'. Which one should we use?

---

**👤 You:**
> "Run the 'Ghost Mannequin' workflow (ID: 'wf_123') on image ID 'img_456'."

**🤖 AI Agent:**
> Execution triggered! I've started processing image img_456 using the specified workflow. The execution ID is 'exec_789'. I'll monitor the status and notify you when the high-fidelity result is ready.

---

**👤 You:**
> "Check status and get the result URL for execution 'exec_789'."

**🤖 AI Agent:**
> Fetching status... Execution exec_789 is currently 'Success'. You can access your high-fidelity processed image here: [result_url]. Need any help with more batch tasks?


## ❓ FAQ

**Q: How do I find my autoRetouch API credentials?**
Log in to your account, navigate to the API section to generate an Access Token (Bearer), and find your Organization ID in the organization settings.

**Q: Can I process multiple images at once?**
Yes! You can trigger individual executions programmatically and group them into a single batch for high-fidelity tracking.

**Q: What happens if a process fails?**
The `get_execution_status` tool will return high-fidelity error metadata to help you diagnose and re-run the task programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/autoretouch](https://vinkius.com/mcp/autoretouch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **autoRetouch** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `autoretouch` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **autoRetouch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "autoretouch": {
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
