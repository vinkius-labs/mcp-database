# Urlbox MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/urlbox-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/urlbox-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/urlbox-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Render websites as high-quality screenshots and PDFs with a cloud API that handles responsive layouts and dynamic content.

## Description
Connect your **Urlbox** account to any AI agent and simplify how you generate high-quality website screenshots, PDF conversions, and HTML renders through natural conversation.

### What you can do

- **Web Capture** — Generate instant screenshots of any public URL in multiple formats (PNG, JPG, WebP, SVG).
- **PDF Conversion** — Convert entire webpages to high-fidelity PDF documents with customizable page sizes.
- **HTML Rendering** — Render raw HTML code directly into images to test styles or generate dynamic assets.
- **Selective Capture** — Use CSS selectors to capture only specific elements of a page (e.g., just a chart or a header).
- **Usage Monitoring** — Track your credit balance and monthly usage stats directly from your agent.
- **Technical Insights** — Retrieve active webhooks, storage buckets, and available proxy locations for premium rendering.

### How it works

1. Subscribe to this server
2. Enter your Urlbox API Key (found in your account dashboard)
3. Start capturing the web from Claude, Cursor, or any MCP client

### Who is this for?

- **Web Developers & Designers** — quickly verify responsive layouts and render HTML snippets via simple AI commands.
- **Marketing Teams** — automate the collection of visual proofs for ads and social media landing pages.
- **Content Creators** — generate high-quality screenshots and PDF backups of online articles instantly.


## Available Tools
- **get_account_info**: Get account profile
- **list_proxies**: List available proxies
- **get_render_status**: Check render status
- **get_credit_usage**: Get usage stats
- **list_storage_buckets**: List storage buckets
- **list_webhooks**: List active webhooks
- **render_async**: Result is sent to webhook.

Render URL (Async)
- **render_html**: Render raw HTML
- **capture_pdf**: Convert URL to PDF
- **capture_png**: Capture PNG screenshot
- **render_selector**: Render specific element
- **render_sync**: Render URL (Sync)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Urlbox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Take a high-quality screenshot of 'https://vinkius.com'."

**🤖 AI Agent:**
> Screenshot captured! I've rendered 'https://vinkius.com' as a high-quality PNG. You can view or download the image here: [Render URL]. Shall I convert this page to PDF as well?

---

**👤 You:**
> "Convert the article at 'https://example.com/blog/1' to an A4 PDF."

**🤖 AI Agent:**
> Conversion successful! I've generated an A4 PDF for the provided URL. Here is your download link: [PDF URL]. Is there anything else you'd like to capture?

---

**👤 You:**
> "Capture only the element '#pricing-table' from 'https://mysaas.com'."

**🤖 AI Agent:**
> Selective render complete! I've captured only the element matching '#pricing-table' from 'https://mysaas.com'. Here is the cropped image: [Element URL].


## Installation & Usage

To install and use the **Urlbox** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/urlbox-alternative](https://vinkius.com/mcp/urlbox-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
