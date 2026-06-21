# Netlify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/netlify)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/netlify-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/netlify-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage your Netlify sites and deployments via the Netlify API — list sites, trigger builds, and monitor forms directly from any AI agent.

## Description
Connect your **Netlify** account to any AI agent and orchestrate your web hosting and deployment workflows through natural conversation.

### What you can do

- **Site Oversight** — List and retrieve detailed information for all your web projects hosted on Netlify.
- **Deployment Management** — Monitor deploy statuses and retrieve specifics for any historical deployment.
- **Build Automation** — Trigger new builds for your sites directly from your workspace.
- **Form Processing** — Access form submissions and list available forms to monitor user engagement.
- **DNS & Domains** — List managed DNS zones and domains associated with your account.
- **User Insights** — Retrieve authenticated user profile information for account verification.

### How it works

1. Subscribe to this server
2. Enter your Netlify Personal Access Token
3. Start managing your edge-native sites from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Frontend Developers** — quickly check deploy statuses and trigger builds without leaving their editor.
- **DevOps Engineers** — monitor site health and domain configurations straight from their workflow tools.
- **Content Teams** — retrieve recent form submissions and user feedback using natural language.


## Available Tools
- **get_deploy**: Get specific deploy details
- **get_site**: Get details of a specific site
- **get_user**: Get authenticated user profile
- **list_domains**: List all DNS zones/domains
- **list_builds**: List builds for a site
- **list_deploys**: List all deploys for a site
- **list_form_submissions**: List submissions for a specific form
- **list_forms**: List all forms for a site
- **list_sites**: List all Netlify sites
- **trigger_build**: Trigger a new build for a site


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Netlify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Netlify sites."

**🤖 AI Agent:**
> I've retrieved your sites. You have 3 projects active: 'Portfolio V2' (ID: site_1), 'Company Blog' (ID: site_2), and 'E-commerce App' (ID: site_3).

---

**👤 You:**
> "Trigger a new build for site site_1."

**🤖 AI Agent:**
> Triggering the build for 'Portfolio V2'... Done! A new build process has started. You can monitor its progress using `list_builds`.

---

**👤 You:**
> "Show the latest contact form submissions for site_2."

**🤖 AI Agent:**
> Retrieving form submissions... I found 3 recent messages. Topics include 'Pricing Inquiry' from John and 'Technical Issue' from Sarah. Would you like to see the full content of these messages?


## Installation & Usage

To install and use the **Netlify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/netlify](https://vinkius.com/mcp/netlify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
