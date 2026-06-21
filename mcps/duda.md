# Duda MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/duda)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/duda-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/duda-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage websites, track templates, and monitor client accounts via the Duda API.

## Description
Integrate **Duda**, the professional website builder for agencies and SaaS, directly into your AI workflow. Manage your fleet of websites and their publishing statuses, track available site templates, monitor client accounts and permissions, and oversee dynamic data collections using natural language.

### What you can do

- **Website Oversight** — List and retrieve detailed configuration and real-time status for all your Duda websites and domains.
- **Template Intelligence** — Access the Duda template library to monitor available designs and structural organizational identifiers.
- **Client Management** — Track client account profiles, email addresses, and individual permissions across your organization.
- **Collection Monitoring** — List dynamic data collections associated with specific sites to ensure efficient content management.

### How it works

1. Connect the Duda integration to your AI assistant.
2. Authorize using your Duda API Username and Password (found in your developer portal).
3. Orchestrate your website management and agency operations through intuitive conversation.

### Who is this for?

- **Agency Managers** — Quickly check site publishing statuses and client volumes on the go.
- **Web Developers** — Audit site configurations and dynamic collections via chat.
- **Operations Teams** — Monitor template usage and client access permissions across the organization instantly.


## Available Tools
- **search_sites_by_domain**: Search for a Duda site using a domain or name keyword
- **get_template_details**: Get detailed information for a specific Duda template
- **list_client_accounts**: List all client accounts registered in your Duda organization
- **list_site_collections**: List all dynamic data collections associated with a specific site
- **list_published_websites**: Identify sites that are currently in a "Published" status
- **list_duda_sites**: List all websites configured in your Duda account
- **list_site_templates**: List all available Duda website templates
- **get_client_account_profile**: Get full profile and permission data for a specific client account
- **quick_site_health_audit**: Retrieve a high-level summary of site activity and publishing rates
- **get_site_details**: Get detailed settings and information for a specific Duda site


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Duda** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my published Duda sites."

**🤖 AI Agent:**
> I've found 12 published sites, including 'Main Corporate Site' (corporate.com) and 'E-commerce Shop' (shop.com). Would you like to see the creation date for any of these?

---

**👤 You:**
> "Show me the details for site 'site_12345'."

**🤖 AI Agent:**
> Site 'site_12345' (Name: Tech Project) is currently 'PUBLISHED'. It is using the 'Modern Agency' template and has 2 dynamic collections. Should I list the collections for this site?

---

**👤 You:**
> "Which client accounts have permission to 'Manage Blog'?"

**🤖 AI Agent:**
> In your organization, 3 client accounts have 'Manage Blog' permissions: 'John Doe', 'Alice Miller', and 'Marketing Team A'. Would you like to see the full profile for John Doe?


## Installation & Usage

To install and use the **Duda** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/duda](https://vinkius.com/mcp/duda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
