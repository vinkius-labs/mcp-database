# Capsulink MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/capsulink)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/capsulink-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/capsulink-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage shortened URLs via Capsulink — create links, track clicks, and monitor analytics directly from any AI agent.

## Description
Connect your **Capsulink** account to any AI agent and orchestrate your link shortening, click tracking, and digital marketing workflows through natural conversation.

### What you can do

- **Link Oversight** — List all your shortened links and retrieve detailed metadata, including destination URLs and creation dates.
- **Performance Tracking** — Retrieve total and daily click statistics for specific links to monitor engagement.
- **Dynamic Redirection** — Change the destination URL of an existing link instantly without changing the short back-half.
- **Link Organization** — Access and list your link folders to maintain a structured marketing assets library.
- **Operational Control** — Delete shortened links permanently directly from your workspace.
- **Quick Shortening** — Create new short links with custom back-halves and titles using natural language.

### How it works

1. Subscribe to this server
2. Enter your Capsulink API Key
3. Start optimizing your links from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Digital Marketers & SMMs** — quickly shorten links for campaigns or check click counts without manual dashboard work.
- **Growth Engineers** — automate link creation and redirection straight from their workflow tools.
- **Business Admins** — monitor link performance and account health using natural language.


## Available Tools
- **delete_link**: Delete a shortened link permanently
- **edit_link_destination**: Change the destination URL of an existing shortened link
- **get_account_info**: Retrieve core account information
- **get_link_daily_stats**: Retrieve daily click breakdown for a specific link
- **get_link_details**: Get basic details of a specific shortened link
- **get_link_stats**: Retrieve total click statistics for a specific link
- **list_link_folders**: List all folders used to organize links
- **list_links**: List all shortened links in your account
- **shorten_url**: Shorten a long URL using Capsulink


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Capsulink** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Shorten https://vinkius.com/blog/new-feature with title 'Blog Feature'."

**🤖 AI Agent:**
> I've shortened the URL. Your new link is https://clnk.to/abcde (ID: cap_123).

---

**👤 You:**
> "Show click stats for link with ID cap_123."

**🤖 AI Agent:**
> Link cap_123 ('Blog Feature') has received 450 total clicks since it was created on March 15th.

---

**👤 You:**
> "Change the destination of link cap_123 to https://vinkius.com/pricing."

**🤖 AI Agent:**
> The destination URL for link cap_123 has been successfully updated to the pricing page.


## Installation & Usage

To install and use the **Capsulink** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/capsulink](https://vinkius.com/mcp/capsulink)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
