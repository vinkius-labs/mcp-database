# cloudlayer.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudlayerio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cloudlayerio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cloudlayerio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate PDFs and screenshots via cloudlayer.io — convert HTML or URLs to high-quality documents and images directly from any AI agent.

## Description
Connect your **cloudlayer.io** account to any AI agent and take full control of your document and image generation through natural conversation. Streamline how you create pixel-perfect PDFs and website screenshots natively.

### What you can do

- **PDF Generation** — Convert public URLs or raw HTML strings into high-quality PDF documents natively
- **Screenshot Intelligence** — Capture high-resolution screenshots of any web page in PNG, JPG, or WebP formats flawlessly
- **Template Management** — List and retrieve details for Nunjucks templates configured in your account flawlessly
- **Generation History** — Access a history of recent document and image generation tasks to track activity flawlessly
- **Usage Auditing** — Retrieve current usage statistics and quota information directly within your workspace securely
- **Webhook Logistics** — Monitor all configured webhooks for real-time generation notifications flawlessly

### How it works

1. Subscribe to this server
2. Enter your cloudlayer.io API Key (obtained from your dashboard)
3. Start generating PDFs and screenshots from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Automation Teams** — automate PDF reports and social media preview images using natural language
- **Developers** — audit document generation status and verify template configurations without opening the dashboard
- **Marketing Specialists** — quickly capture website snapshots and create thumbnails straight from their chat interface
- **Compliance Teams** — verify usage quotas and monitor document generation history


## Available Tools
- **convert_html_to_pdf**: Convert raw HTML string into a PDF document
- **capture_url_screenshot**: Capture a high-quality screenshot (image) of a public URL
- **convert_url_to_pdf**: Convert a public URL into a high-quality PDF document
- **get_template_configuration**: Get details for a specific generation template
- **get_cloudlayer_usage_stats**: Retrieve current usage and quota information
- **list_generation_history**: List recent document and image generation history
- **list_pdf_templates**: List all Nunjucks templates configured in the account
- **list_cloudlayer_webhooks**: List all configured webhooks for async notifications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **cloudlayer.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert https://example.com to a PDF."

**🤖 AI Agent:**
> Generating PDF for example.com... The document has been successfully created. You can download it here: [Generated PDF URL].

---

**👤 You:**
> "Take a screenshot of https://news.google.com."

**🤖 AI Agent:**
> Capturing screenshot of Google News... I've generated a high-quality image of the page. You can view it here: [Screenshot URL].

---

**👤 You:**
> "Show me my generation history."

**🤖 AI Agent:**
> Retrieving your history... I found 5 recent tasks including 3 PDFs from URLs, 1 HTML conversion, and 1 screenshot. Would you like the links for any of these?


## Installation & Usage

To install and use the **cloudlayer.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudlayerio](https://vinkius.com/mcp/cloudlayerio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
