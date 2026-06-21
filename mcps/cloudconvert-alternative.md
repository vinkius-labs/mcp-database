# CloudConvert MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudconvert-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Convert files between 200+ formats including PDF, images, video, and documents with a fast cloud-based processing engine.

## Description
Connect your **CloudConvert** account to any AI agent and take full control of your cloud-based file processing and document automation workflows through natural conversation.

### What you can do

- **Multimodal Conversion Orchestration** — Convert files between 200+ supported formats, including video (MP4, MKV), audio (MP3, WAV), documents (PDF, DOCX), and images programmatically
- **Job & Task Architecture** — Create and manage complex conversion jobs with multiple tasks (import, convert, export) to coordinate high-fidelity processing pipelines
- **Automated Workflow** — Programmatically import files from public URLs and retrieve secure download links for the finalized converted assets
- **Administrative Visibility** — Monitor your account profile, remaining credits, and conversion progress in real-time directly through your agent
- **Format Intelligence** — Retrieve complete directories of supported conversion formats and import/export operations to ensure the perfect processing strategy

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the CloudConvert dashboard (Dashboard > API)
3. Set the **'Use Sandbox'** option to 'true' for testing without consuming credits
4. Start automating your file processing from Claude, Cursor, or any MCP client

No more manual file uploading or searching for specialized converter apps. Your AI acts as your dedicated document engineer and media production coordinator.

### Who is this for?

- **Developers & Engineers** — instantly automate on-the-fly file processing and document workflows using natural language commands
- **Content Creators** — convert media assets between high-fidelity formats without leaving your creative workspace
- **Operations Leads** — automate bulk document conversions and monitor credit utilization through simple AI queries


## Available Tools
- **cancel_job**: Cancel a conversion job
- **create_simple_job**: Create a simple conversion job (URL to Output format)
- **get_job**: Get details of a specific job
- **get_task**: Get details of a specific task
- **get_task_status**: Check the status of a specific task
- **get_user**: Get current user profile and credits
- **list_conversion_formats**: List supported conversion formats
- **list_export_operations**: List supported export operations
- **list_import_operations**: List supported import operations
- **list_jobs**: List all conversion jobs
- **list_tasks**: List all tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CloudConvert** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert the DOCX file at 'https://example.com/spec.docx' to PDF."

**🤖 AI Agent:**
> Conversion job triggered! I've started the process to convert your DOCX specification into a high-fidelity PDF. The job ID is 'job_123'. I'll retrieve the secure download link for you once it's ready.

---

**👤 You:**
> "List my last 5 conversion jobs and their statuses."

**🤖 AI Agent:**
> I've retrieved your recent jobs. Highlights include a successful MP4 to MKV conversion (ID: job_402) and two completed PDF exports. Would you like the download links for any of these finalized files?

---

**👤 You:**
> "Check my remaining CloudConvert credits."

**🤖 AI Agent:**
> Scanning account... You currently have 1,240 conversion credits remaining in your profile. Your connection is active and healthy. Need help starting a new high-fidelity media conversion?


## ❓ FAQ

**Q: How do I find my CloudConvert API Key?**
Log in to your account, navigate to the **Dashboard**, click on **API** in the sidebar, and generate or copy your secret key.

**Q: Which formats are supported for conversion?**
CloudConvert supports over 200 formats including PDF, DOCX, XLSX, MP4, MKV, MP3, JPG, PNG, and many more.

**Q: What is the 'Sandbox' mode?**
The Sandbox is a testing environment that allows you to run conversion jobs for free. Note that files processed in Sandbox are not actual conversions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudconvert-alternative](https://vinkius.com/mcp/cloudconvert-alternative)
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
3. Set Type to "SSE", enter `cloudconvert-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CloudConvert** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloudconvert-alternative": {
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
