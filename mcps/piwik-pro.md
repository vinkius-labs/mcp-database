# Piwik PRO MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/piwik-pro)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/piwik-pro-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/piwik-pro-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage privacy-first analytics via Piwik PRO — list apps, execute custom queries, and monitor goals directly from any AI agent.

## Description
Connect your **Piwik PRO Analytics Suite** to any AI agent and take full control of your privacy-compliant data workflows through natural conversation.

### What you can do

- **Analytics Discovery** — List all websites and apps (containers) tracked in your Piwik PRO account.
- **Custom Reporting** — Execute complex analytics queries using JSON to extract specific dimensions and metrics.
- **Goal Tracking** — List and monitor conversion goals for any specific application.
- **Dashboard Visibility** — List available dashboards to maintain an overview of your analytical insights.
- **Admin Oversight** — List account users and tracking sites to manage your organization's setup.

### How it works

1. Subscribe to this server
2. Enter your Piwik PRO Client ID, Client Secret, and Subdomain
3. Start analyzing your data directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Privacy Officers** — quickly verify tracking sites and user access levels to ensure compliance.
- **Digital Analysts** — execute custom queries and audit goal conversions without leaving the IDE.
- **Marketing Managers** — monitor high-level dashboard metadata and application lists through simple chat commands.


## Available Tools
- **list_piwik_apps**: List all websites/apps in Piwik PRO
- **list_piwik_dashboards**: List Piwik PRO dashboards
- **list_piwik_goals**: List goals for a specific app
- **list_piwik_sites**: List tracking sites
- **list_piwik_users**: List account users
- **query_piwik_analytics**: Requires a JSON query body.

Execute a custom analytics query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Piwik PRO** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all websites tracked in my Piwik PRO account."

**🤖 AI Agent:**
> I've retrieved your apps. You have 3 tracked sites: 'Main Corporate Site', 'E-commerce Portal', and 'Customer Help Center'. Would you like to see the conversion goals for any of these?

---

**👤 You:**
> "What are the conversion goals defined for the 'E-commerce Portal' (ID: 12345)?"

**🤖 AI Agent:**
> There are 4 goals defined for this portal: 'Completed Purchase', 'Added to Cart', 'Newsletter Signup', and 'Contact Form Submission'.

---

**👤 You:**
> "List all users with access to our Piwik PRO organization."

**🤖 AI Agent:**
> I've retrieved the user list. There are 8 users with various roles, including 2 Administrators, 4 Editors, and 2 Viewers.


## Installation & Usage

To install and use the **Piwik PRO** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/piwik-pro](https://vinkius.com/mcp/piwik-pro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
