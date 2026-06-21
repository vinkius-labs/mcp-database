# CloudConvert MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudconvert)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage file conversions via CloudConvert — track jobs, monitor tasks, and automate file processing directly from any AI agent.

## Description
Connect your **CloudConvert** account to any AI agent and take full control of your file conversion and processing through natural conversation. Streamline how you transform over 200 formats including PDF, DOCX, and more.

### What you can do

- **Job Oversight** — Create and retrieve details for complex file processing jobs with multiple tasks natively
- **Conversion Intelligence** — Access status and results for specific tasks flawlessly to handle async workflows
- **Multi-format Logistics** — Automate conversions between hundreds of different file formats securely
- **Account Visibility** — Retrieve information about your authenticated user profile and remaining credits flawlessly
- **Operation Auditing** — List available AI-powered operations like optimization and website capture securely
- **Webhook Logistics** — Monitor configured webhooks for real-time job completion notifications directly within your workspace flawlessly

### How it works

1. Subscribe to this server
2. Enter your CloudConvert API Key (obtained from Dashboard > API v2)
3. Start converting your files from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — automate image and video conversions using natural language
- **Developers** — audit conversion job statuses and verify task outputs without opening the dashboard
- **Office Teams** — quickly transform documents and optimize PDFs straight from their chat interface
- **Automation Specialists** — verify webhook delivery and monitor conversion quotas


## Available Tools (8)
- **create_conversion_job**: Supports over 200 formats.

Create a new file conversion or processing job
- **get_conversion_job_details**: Get the status and result of a specific job
- **get_my_cloudconvert_profile**: Retrieve information about the authenticated user and credits
- **get_conversion_task_details**: Get detailed information for a specific task
- **list_conversion_jobs**: List all recent conversion jobs
- **list_available_conversion_ops**: List common operations supported by the CloudConvert API
- **list_conversion_tasks**: List all individual tasks across jobs
- **list_cloudconvert_webhooks**: List configured webhooks for job completion notifications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CloudConvert** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 conversion jobs in CloudConvert."

**🤖 AI Agent:**
> Retrieving your recent jobs... I found 5 items including 'invoice-pdf', 'profile-image-optimize', and 'video-transcode'. All are currently in 'finished' status.

---

**👤 You:**
> "What is the status of conversion task 'task_12345'?"

**🤖 AI Agent:**
> Checking status for task_12345... The task is 'finished'. You can download the result from this URL: [Download URL].

---

**👤 You:**
> "How many credits do I have left in CloudConvert?"

**🤖 AI Agent:**
> Checking your account balance... You currently have 450 credits remaining in your CloudConvert account. This covers approximately 450 minutes of conversion time.


## ❓ FAQ

**Q: Can I convert a document to PDF through the agent?**
Yes! Use the `create_conversion_job` tool. You can define an import task for your file and a convert task with `output_format: 'pdf'`. The agent will handle the submission to CloudConvert.

**Q: How do I know when my conversion task is finished?**
Use the `get_conversion_task_details` tool with your task ID. Your agent will return the current status, and once it shows 'finished', it will provide the download URL.

**Q: Where do I find my CloudConvert API Key?**
Log in to your CloudConvert dashboard and navigate to **API v2 > API Keys**. You can generate and copy your personal API key from there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudconvert](https://vinkius.com/mcp/cloudconvert)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CloudConvert** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cloudconvert` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CloudConvert** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloudconvert": {
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
