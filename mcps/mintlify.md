# Mintlify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mintlify)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mintlify-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mintlify-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage and automate your Mintlify documentation—retrieve metadata, update configurations, track page views, and trigger deployments directly from your AI agent.

## Description
Connect your **Mintlify** account to any AI agent to streamline your documentation workflow through natural conversation.

### What you can do

- **Metadata Management** — Retrieve your project's current settings, navigation structure, and configuration via `get_metadata`.
- **Configuration Updates** — Modify your documentation's configuration object programmatically using `update_metadata`.
- **Analytics Tracking** — Monitor documentation performance by fetching page view statistics for specific time ranges with `get_page_views`.
- **Deployment Triggers** — Instantly trigger new deployments of your documentation using `trigger_deployment`, perfect for CI/CD workflows.

### How it works

1. Subscribe to this server
2. Enter your Mintlify API Key
3. Start managing your technical documentation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — trigger deployments and update configurations directly from the code editor.
- **Technical Writers** — inspect navigation structures and metadata without leaving the chat interface.
- **Product Managers** — quickly check documentation traffic and analytics to understand user engagement.


## Available Tools
- **get_metadata**: Get Mintlify project metadata
- **get_page_views**: Get Mintlify page views analytics
- **trigger_deployment**: This is useful for CI/CD integrations.

Trigger a new Mintlify deployment
- **update_metadata**: Update Mintlify project metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mintlify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the current metadata for my Mintlify project."

**🤖 AI Agent:**
> I've retrieved your project metadata. Your documentation is currently configured with the navigation structure including 'Introduction', 'API Reference', and 'Guides'. Would you like to see the full JSON configuration?

---

**👤 You:**
> "Show me the page views for the last 30 days."

**🤖 AI Agent:**
> Fetching analytics... In the last 30 days, your documentation received a total of 12,450 page views. The most visited page was '/api-reference/authentication'.

---

**👤 You:**
> "Trigger a new deployment for my documentation."

**🤖 AI Agent:**
> Deployment triggered successfully! Mintlify is now building the latest version of your documentation. You can check the status in your dashboard.


## Installation & Usage

To install and use the **Mintlify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mintlify](https://vinkius.com/mcp/mintlify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
