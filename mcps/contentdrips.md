# Contentdrips MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contentdrips)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/contentdrips-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/contentdrips-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Turn text into scroll-stopping social media carousels and visual content pieces that boost engagement on every platform.

## Description
Connect your **Contentdrips** account to any AI agent and take full control of your automated social media graphic generation and carousel publishing through natural conversation.

### What you can do

- **Graphic Portfolio Orchestration** — Programmatically trigger social media renders (Carousels, Quote Graphics) using custom text and image inputs
- **Job & Status Intelligence** — Programmatically monitor real-time generation statuses (Pending, Processing, Completed) to maintain a perfectly coordinated content pipeline
- **Asset & Output Monitoring** — Access hosted render URLs (PNG, PDF) and retrieve technical metadata for your social media archive in real-time
- **Template Discovery** — Programmatically retrieve technical Template IDs from your account to oversee your organizational design ecosystem
- **Operational Monitoring** — Verify account-level API connectivity and monitor rendering volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Contentdrips dashboard (Settings > API)
3. Start orchestrating your social content from Claude, Cursor, or any MCP client

No more manual designing of individual carousel slides or missing scheduled content slots. Your AI acts as your dedicated graphic coordinator and content architect.

### Who is this for?

- **Social Media Managers** — instantly trigger carousel renders and monitor job status using natural language commands
- **Content Creators** — verify individual graphic metadata and track render history without leaving your creative workspace
- **Growth Engineers** — automate the ingestion of high-speed Contentdrips assets into custom scheduling tools through simple AI queries


## Available Tools
- **check_contentdrips_status**: Verify ContentDrips API connectivity
- **get_account**: Get account info
- **get_job_result**: Get render result
- **get_job_status**: Check render job status
- **get_template**: Get template details
- **list_templates**: List all templates
- **render_batch**: Render a batch of graphics
- **render_carousel**: Render a carousel
- **render_image**: Render a single image
- **render_pdf**: Render as PDF


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contentdrips** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Render a carousel with template '148872' and text: 'Top 5 AI Tools'."

**🤖 AI Agent:**
> Render orchestrated! I've successfully submitted the generation request for template 148872. The job ID is job_abc123. The carousel will be ready shortly. Shall I notify you once the status is 'Completed'?

---

**👤 You:**
> "Check the status of render job 'job_abc123'."

**🤖 AI Agent:**
> Job intelligence orchestrated! For job_abc123, the current status is 'COMPLETED'. The asset was generated successfully at 2:00 PM today. Need help retrieving the final export URL?

---

**👤 You:**
> "Retrieve the final PNG URL for job 'job_abc123'."

**🤖 AI Agent:**
> Asset directory orchestrated! I've successfully retrieved the PNG URL for job_abc123. The image is now ready for your social media schedule. Shall I list the technical metadata for this render?


## Installation & Usage

To install and use the **Contentdrips** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contentdrips](https://vinkius.com/mcp/contentdrips)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
