# Dopplio MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dopplio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dopplio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dopplio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Send personalized video messages at scale that use AI to customize each clip for the recipient and boost response rates.

## Description
Connect your **Dopplio** account to any AI agent and take full control of your multimedia automation and document rendering workflows through natural conversation.

### What you can do

- **AI Video Orchestration** — Start and manage asynchronous video generation tasks using advanced lipsync and voice cloning technology programmatically
- **Document Architecture** — Programmatically generate high-fidelity PDF documents from HTML strings or public URLs for immediate reporting and invoicing
- **Visual Intelligence** — Capture automated screenshots of any website with customizable viewports and formats to monitor web assets or create content
- **Workflow Monitoring** — Track the real-time status of your multimedia rendering jobs to maintain high-fidelity operational transparency
- **Library Visibility** — Access your complete directory of generated videos and retrieve detailed metadata and hosting links directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the Dopplio/Doppio.sh dashboard
3. Start generating AI-powered multimedia from Claude, Cursor, or any MCP client

No more manual document exporting or complex video rendering pipelines. Your AI acts as your dedicated multimedia producer and document coordinator.

### Who is this for?

- **Marketing Operations** — instantly generate personalized video campaigns and dynamic PDF reports using natural language commands
- **Growth Engineers** — automate website monitoring with scheduled screenshots and document generation without leaving your workspace
- **Content Teams** — leverage AI to scale high-engagement video assets and visual summaries through simple AI queries


## Available Tools
- **capture_screenshot**: Capture a website screenshot
- **generate_video**: Provide template and personalization data.

Generate AI-personalized video
- **get_render_status**: Check status of a render job
- **get_video_details**: Get specific video details
- **list_videos**: List all generated videos
- **render_pdf**: Provide "url" or "html" in the JSON body.

Render a PDF from URL or HTML


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dopplio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Render a PDF from the URL 'https://vinkius.com/report'."

**🤖 AI Agent:**
> PDF rendering triggered! I've successfully initiated the document generation for your URL. You can download the finalized file here: [download_url]. Your report is now ready.

---

**👤 You:**
> "Capture a mobile screenshot of 'google.com'."

**🤖 AI Agent:**
> Screenshot captured! I've used the mobile viewport settings to capture 'google.com'. You can view your image here: [image_url]. Shall I check the PDF version of this page as well?

---

**👤 You:**
> "Check the status of my video rendering job 'job_123'."

**🤖 AI Agent:**
> Monitoring job... Video rendering for job_123 is currently 'Completed'. You can now access the hosting URL and metadata. Shall I retrieve the direct download link for you?


## Installation & Usage

To install and use the **Dopplio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dopplio](https://vinkius.com/mcp/dopplio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
