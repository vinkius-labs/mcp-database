# Browserbase MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/browserbase)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/browserbase-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/browserbase-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Cloud browser infrastructure for AI agents — create, control, and manage headless Chromium sessions via CDP for automated web interaction.

## Description
Connect your AI agent to **Browserbase** — the serverless platform for running headless cloud browsers at scale.

### What you can do

- **Create Sessions** — Spin up isolated Chromium browser sessions in the cloud. Each session returns a CDP (Chrome DevTools Protocol) WebSocket URL for connecting Playwright, Puppeteer, or Selenium
- **List Sessions** — Monitor all active, completed, or errored browser sessions across your account
- **Get Session Details** — Check status, connection URLs, pages visited, and duration of any session
- **Stop Sessions** — Terminate running sessions to free resources

### How it works

1. Subscribe to this server
2. Enter your Browserbase API key (1 free browser hour included)
3. Your agent can now launch and control real browsers in the cloud

### Who is this for?

- **AI Agent Developers** — give agents a real browser for complex interactions (login, click, fill forms, navigate SPAs)
- **QA Automation** — run browser-based tests at scale without infrastructure
- **Web Scraping** — access content that requires JavaScript execution, authentication, or complex navigation


## Available Tools
- **create_browser_session**: The session provides a connectUrl (CDP WebSocket) that can be used with Playwright, Puppeteer, or Selenium to control the browser programmatically. Default timeout is 300 seconds.

Create a new cloud browser session. Returns a CDP WebSocket URL for connecting automation frameworks like Playwright or Puppeteer
- **get_browser_session**: Useful for monitoring active sessions.

Get details of a specific browser session by its ID
- **list_browser_sessions**: Filter by status: RUNNING, COMPLETED, ERROR.

List all active browser sessions in your Browserbase account
- **stop_browser_session**: Any unsaved state in the browser is lost.

Stop a running browser session by its ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Browserbase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new browser session so I can automate a login flow."

**🤖 AI Agent:**
> Browser session created!

| Session ID | Status | Region | Info |
|---|---|---|---|
| `sess_abc123` | created | us-west-2 | Browser: chromium |

**Connect URL:** `wss://connect.browserbase.com/sess_abc123`

Use this WebSocket URL with Playwright or Puppeteer to control the browser.

---

**👤 You:**
> "Show me all my running browser sessions."

**🤖 AI Agent:**
> Found 2 active sessions:

| Session ID | Status | Region | Info |
|---|---|---|---|
| `sess_abc123` | running | us-west-2 | Pages: 3, Duration: 2min |
| `sess_def456` | running | us-east-1 | Pages: 1, Duration: 30s |

---

**👤 You:**
> "Stop browser session sess_abc123."

**🤖 AI Agent:**
> Session stopped!

| Session ID | Status | Info |
|---|---|---|
| `sess_abc123` | stopped | Session terminated — resources released |


## Installation & Usage

To install and use the **Browserbase** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browserbase](https://vinkius.com/mcp/browserbase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
