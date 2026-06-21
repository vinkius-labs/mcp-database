# Rebrandly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rebrandly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rebrandly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rebrandly-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Link management platform to create and manage branded short URLs with AI.

## Description
### What you can do
- Create and manage branded short links with custom slashtags to enhance your brand presence and track performance.
- Organize your links across different workspaces and domains to maintain a structured marketing ecosystem.
- Update destination URLs, titles, and metadata programmatically to adapt to changing marketing campaigns.
- Access real-time click statistics and account metadata through the Rebrandly REST API v1.

### How it works
1. Retrieve your API Key from your Rebrandly account (Account > API).
2. Optionally provide a Workspace ID to manage links within specific team environments.
3. Connect your AI agent to automate link generation, campaign tracking, and branding workflows.

### Who is it for?
Designed for digital marketers, brand managers, and developers who want to leverage AI for intelligent link management and high-fidelity branding automation.


## Available Tools
- **get_link_count**: Check link usage
- **create_branded_link**: Shorten a URL
- **delete_short_link**: Remove a link
- **get_account_details**: Get profile info
- **get_domain_info**: Get domain metadata
- **get_link_details**: Get link info
- **list_branded_domains**: List custom domains
- **list_short_links**: List branded links
- **list_account_workspaces**: List team spaces
- **search_links_by_title**: Find links
- **test_rebrandly_auth**: Check connection
- **update_link_metadata**: Modify a link


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rebrandly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a branded link for our new summer collection landing page at https://fashion-hub.com/collections/summer-2024 and use the slashtag 'summer-vibes'."

**🤖 AI Agent:**
> Successfully created your branded link: https://fshn.link/summer-vibes. It is now active and ready to be shared in your marketing campaigns.

---

**👤 You:**
> "How many branded links have we generated in our account so far?"

**🤖 AI Agent:**
> You have generated a total of 1,248 branded links across your current workspace.

---

**👤 You:**
> "Find the link titled 'Q3 Investor Update' and update its destination to https://investors.techcorp.com/reports/q3-final."

**🤖 AI Agent:**
> I found the link 'Q3 Investor Update' and successfully updated its destination URL to the new report location.


## Installation & Usage

To install and use the **Rebrandly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rebrandly](https://vinkius.com/mcp/rebrandly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
