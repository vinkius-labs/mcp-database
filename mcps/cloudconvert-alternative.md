# CloudConvert MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudconvert-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cloudconvert-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cloudconvert-alternative-mcp)
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


## Installation & Usage

To install and use the **CloudConvert** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudconvert-alternative](https://vinkius.com/mcp/cloudconvert-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
