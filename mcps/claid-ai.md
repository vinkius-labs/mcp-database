# Claid AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/claid-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate AI image processing via Claid — upscale resolution, remove backgrounds, and enhance product photos directly from any AI agent.

## Description
Connect your **Claid AI** account to any AI agent and take full control of your image enhancement workflows through natural conversation. Transform basic product shots into professional photography instantly.

### What you can do

- **AI Enhancement** — Apply multiple enhancements like HDR adjustment, white balance, and polishing natively
- **Resolution Upscaling** — Increase image dimensions using specialized AI models for photos and digital art flawlessly
- **Background Logistics** — Remove or replace backgrounds with white or custom scenes securely
- **Task Oversight** — Monitor the status of async processing tasks and retrieve results flawlessly
- **Canvas Control** — Resize images to specific dimensions with intelligent fit/fill logic flawlessly
- **Account Visibility** — Retrieve core account information and monitor your AI usage quotas directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Claid AI API Key (obtained from your dashboard)
3. Start enhancing your product photos from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — automate product photo editing and background removal using natural language
- **Marketplace Sellers** — upscale low-resolution images to meet professional standards without manual work
- **Graphic Designers** — quickly verify AI processing results and task statuses straight from their chat interface
- **Developers** — integrate high-quality AI image editing into marketplace pipelines


## Available Tools (8)
- **list_claid_collections**: List image collections in your account
- **list_available_ai_operations**: List common AI operations supported by the Claid API
- **enhance_image**: You can combine multiple operations like upscale, background removal, and HDR adjustment.

Apply AI enhancements and edits to an image
- **remove_image_background**: Quickly remove or replace the background of an image
- **upscale_image_resolution**: Increase image resolution using AI models
- **get_claid_account_info**: Retrieve core account and quota information
- **get_processing_task_details**: Get the status and result of an async image processing task
- **list_claid_webhooks**: List configured webhooks for async notifications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claid AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Upscale this product photo to high resolution: https://example.com/shoe.jpg"

**🤖 AI Agent:**
> Initiating upscale for the product photo... I've started the processing task (ID: task_12345). I'll check back in a few seconds to see if your high-resolution image is ready.

---

**👤 You:**
> "Remove the background from this image: https://example.com/model.jpg"

**🤖 AI Agent:**
> Processing background removal for model.jpg... The background has been successfully removed and replaced with white. You can download the result here: [Output URL].

---

**👤 You:**
> "What is the status of processing task 'task_98765'?"

**🤖 AI Agent:**
> Checking status for task_98765... The task is still 'Processing'. Claid AI is currently applying the requested HDR and Polishing adjustments. I'll check again in a moment.


## ❓ FAQ

**Q: Can I upscale an image to 4K resolution through the agent?**
Yes! Use the `upscale_image_resolution` tool. You can specify the model (e.g., `photo` for realistic images) and the agent will instruct Claid AI to enhance the image to high resolution.

**Q: How do I check if my image processing task is finished?**
Use the `get_processing_task_details` tool with the unique task ID. Your agent will fetch the current status and provide the output URL once the processing is complete.

**Q: Where do I find my Claid AI API Key?**
Log in to your Claid.ai dashboard and navigate to the API or Settings section. You can generate and copy your API key from there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/claid-ai](https://vinkius.com/mcp/claid-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claid AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claid-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claid AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claid-ai": {
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
