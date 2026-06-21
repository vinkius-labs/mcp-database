# NameSilo (Domain Registrar Developer API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/namesilo-domain-registrar-developer-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/namesilo-domain-registrar-developer-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/namesilo-domain-registrar-developer-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your domain portfolio, DNS records, and registrations directly through NameSilo's developer API.

## Description
Connect your **NameSilo** account to any AI agent to automate domain management and DNS orchestration. This server provides full access to the NameSilo Developer API, allowing for seamless domain operations within your development workflow.

### What you can do

- **Domain Search & Registration** — Check availability for multiple domains and register them instantly with custom renewal and privacy settings.
- **DNS Management** — List, add, update, or delete DNS records (A, CNAME, MX, TXT, etc.) for any domain in your account.
- **Portfolio & Organization** — List all active domains, organize them into portfolios, and retrieve detailed WHOIS and nameserver information.
- **Account Operations** — Monitor your account balance and add funds to ensure uninterrupted service for your digital assets.
- **Transfers & Renewals** — Initiate domain transfers from other registrars or renew existing registrations for up to 10 years.

### How it works

1. Subscribe to this server
2. Enter your NameSilo API Key
3. Start managing your infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — Automate DNS record updates during deployments or migrations.
- **Domain Investors** — Quickly check availability and manage large portfolios via natural language.
- **Web Developers** — Register domains and configure nameservers without leaving the terminal or code editor.


## Available Tools
- **add_account_funds**: Add funds to your account
- **check_register_availability**: Check if a domain is available for registration
- **contact_add**: Create a new contact profile
- **contact_delete**: Delete a contact profile
- **contact_list**: List all contact profiles
- **contact_update**: Update an existing contact profile
- **dns_add_record**: Add a new DNS record
- **dns_delete_record**: Delete a DNS record
- **dns_list_records**: ) for a domain.

List all DNS records for a domain
- **dns_update_record**: Update an existing DNS record
- **get_account_balance**: Check your account available funds
- **get_domain_info**: Get detailed information about a specific domain
- **list_domains**: Retrieve a list of all domains in your account
- **list_portfolios**: List all domain portfolios
- **portfolio_add**: Create a new portfolio
- **register_domain**: Register a new domain name
- **renew_domain**: Renew an existing domain registration
- **transfer_domain**: Initiate a domain transfer to NameSilo


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NameSilo (Domain Registrar Developer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if 'mcp-server-test.com' and 'mcp-server-test.net' are available."

**🤖 AI Agent:**
> I've checked the availability: 'mcp-server-test.com' is available for $13.95/year, and 'mcp-server-test.net' is available for $12.17/year. Would you like to register either of them?

---

**👤 You:**
> "List all DNS records for my domain 'example.com'."

**🤖 AI Agent:**
> I found 3 DNS records for 'example.com': an A record pointing to 93.184.216.34, and two MX records for mail handling. Do you need to add or update any records?

---

**👤 You:**
> "What is my current NameSilo account balance?"

**🤖 AI Agent:**
> Your current NameSilo account balance is $45.50. You have sufficient funds for upcoming renewals.


## Installation & Usage

To install and use the **NameSilo (Domain Registrar Developer API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/namesilo-domain-registrar-developer-api](https://vinkius.com/mcp/namesilo-domain-registrar-developer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
