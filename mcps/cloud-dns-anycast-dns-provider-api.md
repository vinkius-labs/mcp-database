# Cloud DNS (Anycast DNS Provider API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloud-dns-anycast-dns-provider-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cloud-dns-anycast-dns-provider-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cloud-dns-anycast-dns-provider-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Anycast DNS infrastructure — list zones, configure records, and automate domain management directly through AI.

## Description
Connect your **Cloud DNS** account to any AI agent to manage global Anycast DNS settings through natural language. This server provides direct access to the Cloud DNS API, allowing for rapid deployment and modification of network records.

### What you can do

- **Zone Management** — List all DNS zones and create or delete master/slave zones with specific domain names.
- **Record Control** — Full CRUD operations for A, AAAA, MX, CNAME, TXT, and more within any target zone.
- **Automation & Updates** — Modify existing records, update TTLs, and adjust priorities for MX/SRV records without manual dashboard navigation.
- **Infrastructure Visibility** — Instantly retrieve all records for a specific zone to audit configurations or troubleshoot resolution issues.

### How it works

1. Subscribe to this server
2. Enter your Cloud DNS Auth Key (API Key)
3. Start managing your domains from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate the provisioning of DNS records during CI/CD deployments.
- **System Administrators** — manage global Anycast zones and records via simple text commands.
- **Developers** — quickly point subdomains to new services or update TXT records for domain verification straight from the IDE.


## Available Tools
- **create_record**: Create a new DNS record
- **create_zone**: Create a new DNS zone
- **delete_record**: Delete a DNS record
- **delete_zone**: Delete a DNS zone
- **list_records**: ) within a specific zone.

List all records for a specific zone
- **list_zones**: List all DNS zones
- **update_record**: Update an existing DNS record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloud DNS (Anycast DNS Provider API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my DNS zones."

**🤖 AI Agent:**
> I've retrieved your DNS zones. You have 2 active zones: 'example.com' (ID: 12345) and 'my-app.net' (ID: 67890).

---

**👤 You:**
> "Create a new A record for 'api' pointing to '1.2.3.4' in zone 12345."

**🤖 AI Agent:**
> Successfully created the A record for 'api.example.com' pointing to 1.2.3.4 in zone 12345.

---

**👤 You:**
> "Delete the DNS record with ID 98765 from zone 12345."

**🤖 AI Agent:**
> The DNS record 98765 has been successfully removed from zone 12345.


## Installation & Usage

To install and use the **Cloud DNS (Anycast DNS Provider API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloud-dns-anycast-dns-provider-api](https://vinkius.com/mcp/cloud-dns-anycast-dns-provider-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
