# Browserless MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/browserless)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/browserless-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/browserless-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage headless Chrome via Browserless — take screenshots, generate PDFs, and scrape web content directly from any AI agent.

## Description
Connect your **Browserless.io** account to any AI agent and orchestrate your headless Chrome operations, web automation, and document generation through natural conversation.

### What you can do

- **Visual Captures** — Take high-quality screenshots of any URL with advanced options like full-page capture.
- **Document Generation** — Convert any web page into a polished PDF document directly from your workspace.
- **Rendered Content** — Retrieve the fully rendered HTML content of JavaScript-heavy websites.
- **Custom Scraping** — Run targeted scraping requests by providing element selectors to extract specific data.
- **Infrastructure Monitoring** — Monitor active sessions, retrieve usage statistics, and check the health of the Browserless service.
- **Configuration Access** — Access and verify your account configuration and limits using natural language.

### How it works

1. Subscribe to this server
2. Enter your Browserless.io API Token
3. Start automating web tasks from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web Developers** — quickly debug rendered content or take screenshots for documentation without manual browser work.
- **QA Testers** — automate visual regression captures and session monitoring straight from their workflow tools.
- **Content Managers** — generate PDF versions of web articles or reports using natural language.


## Available Tools
- **check_system_health**: Check the health of the Browserless service
- **generate_pdf**: Generate a PDF of a URL
- **get_account_config**: Retrieve account configuration
- **get_page_content**: Retrieve the rendered HTML content of a URL
- **get_usage_stats**: Retrieve account usage statistics
- **list_active_sessions**: List currently active browser sessions
- **run_scrape**: Run a custom scraping script
- **take_screenshot**: Take a screenshot of a URL using headless Chrome


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Browserless** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Take a full-page screenshot of https://news.ycombinator.com."

**🤖 AI Agent:**
> I've triggered a full-page screenshot for Hacker News. You can view the result here: [Link].

---

**👤 You:**
> "Generate a PDF of the article at https://example.com/blog/post-1."

**🤖 AI Agent:**
> Generating PDF for the article... Your document is ready for download: [Link].

---

**👤 You:**
> "Scrape the titles of all products on https://example.com/shop."

**🤖 AI Agent:**
> Retrieving product titles... I found 12 items, including 'Leather Jacket', 'Denim Jeans', and 'Cotton T-shirt'. Would you like the full list?


## Installation & Usage

To install and use the **Browserless** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browserless](https://vinkius.com/mcp/browserless)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
