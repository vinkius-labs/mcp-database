# Fastly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fastly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fastly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fastly-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage edge computing and CDN via Fastly — monitor and activate service versions, manage domains and backends, and purge cache directly from any AI agent.

## Description
Connect your **Fastly** account to any AI agent and take full control of your edge cloud delivery and CDN configurations through natural conversation.

### What you can do

- **Service Orchestration** — Identify bounded underlying Edge Cloud Delivery mappings and extract CDN service IDs aggregating global payload instances natively
- **Version Management** — Enumerate strictly immutable configuration drafts and promover promoted versions seamlessly to distribute instant security patches
- **Live Traffic Auditing** — Target specific configuration identities evaluating precise Active Version pointers to validate which architectural instance controls live traffic today
- **Edge Deployment** — Deploy drafted VCL or Compute@Edge logic instantly to production by promoting Promoted Drafts to Active states synchronously
- **Cache Purging** — Vaporize the complete Surrogate Cache storing static endpoints globally by issuing absolute HTTP PURGE instructions via chat
- **Backend & Origin Control** — Locate physical upstream Origins (AWS/GCP) mapped inside configurations and verify port constraints shielding original load-balancers
- **Domain Auditing** — Extract precise FQDN apex domains terminated at the Fastly Edge to manage routing configurations for specific headers flawlessly

### How it works

1. Subscribe to this server
2. Enter your Fastly API Token (found in Control Panel > Account > API tokens)
3. Start managing your edge cloud from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SRE Teams** — monitor service versions and trigger cache purges across global points-of-presence using natural language
- **Cloud Architects** — audit backend origin mappings and verify domain configurations without manual dashboard navigation
- **Security Engineers** — deploy instant patches by activating drafted versions and monitor WAF constraints through natural conversation
- **Frontend Developers** — verify CDN configurations and test edge routing logic directly from the IDE or chat


## Available Tools
- **activate_service_version**: Activate a specific configuration version for a service
- **create_service**: Create a new Fastly service
- **delete_service**: Delete a specific Fastly service
- **get_me**: Get current API token identity info
- **get_service**: Get details for a specific Fastly service
- **get_service_stats**: Get usage statistics for a specific service
- **get_service_version**: Get details for a specific service version
- **list_version_backends**: List all backend origins for a specific service version
- **list_version_domains**: List all domains for a specific service version
- **list_services**: List all Fastly services
- **list_service_versions**: List all configuration versions for a service
- **purge_all_cache**: Purge all cached content for a specific service


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fastly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active Fastly services"

**🤖 AI Agent:**
> Retrieving services... I found 3 CDN services: 'Prod-Main-CDN' (ID: 1a2b), 'Staging-App' (ID: 3c4d), and 'Media-Assets' (ID: 5e6f). All are currently terminating traffic across the edge network. Which one would you like to inspect?

---

**👤 You:**
> "Activate version 15 for service 'Prod-Main-CDN'"

**🤖 AI Agent:**
> Version 15 promoted! I've successfully activated the drafted configuration for 'Prod-Main-CDN'. The changes are now live across all global points-of-presence. I'll monitor the traffic health for you.

---

**👤 You:**
> "Purge all cache for service '1a2b'"

**🤖 AI Agent:**
> Cache purge initiated! I've issued a global HTTP PURGE for service 1a2b. All static content has been invalidated, and the network will fetch fresh data from your origins immediately.


## Installation & Usage

To install and use the **Fastly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fastly](https://vinkius.com/mcp/fastly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
