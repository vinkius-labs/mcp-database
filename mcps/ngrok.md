# ngrok MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ngrok)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ngrok-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ngrok-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage ngrok ingress infrastructure — list endpoints, API keys, reserved domains, and security policies directly from your AI agent.

## Description
Connect your **ngrok** account to any AI agent and take full control of your ingress infrastructure through natural conversation.

### What you can do

- **Endpoints & Edges** — List all active public URLs (ephemeral, edge, or cloud) and inspect HTTPS edges for advanced routing configurations
- **Security & Access** — Audit IP policies and restrictions applied to your dashboard, API, or agents to ensure secure access
- **Domain Management** — Retrieve all custom domains reserved for your applications directly from the ngrok cloud
- **Credential Management** — List API keys used for authentication and manage secure vaults for sensitive values
- **Infrastructure Visibility** — Get a bird's-eye view of your entire tunneling setup without leaving your terminal or chat interface

### How it works

1. Subscribe to this server
2. Enter your ngrok API Key
3. Start managing your tunnels and security from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — quickly audit active endpoints and security policies across the organization
- **Backend Developers** — check reserved domains and HTTPS edge configurations during local development
- **Security Teams** — monitor IP restrictions and vault usage to maintain compliance and secure access


## Available Tools
- **list_api_keys**: List ngrok API keys
- **list_endpoints**: List ngrok endpoints
- **list_https_edges**: List ngrok HTTPS edges
- **list_ip_policies**: List ngrok IP policies
- **list_ip_restrictions**: List ngrok IP restrictions
- **list_reserved_domains**: List ngrok reserved domains
- **list_vaults**: List ngrok vaults


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ngrok** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active ngrok endpoints."

**🤖 AI Agent:**
> I've retrieved your active endpoints. You have 2 active tunnels: 'https://myapp.ngrok-free.app' (ID: ep_123) and 'https://api.example.com' (ID: ep_456).

---

**👤 You:**
> "Show me the reserved domains in my account."

**🤖 AI Agent:**
> Fetching reserved domains... I found 3 domains: 'dev.local', 'staging.myapp.com', and 'prod.myapp.com'. All are currently active.

---

**👤 You:**
> "What IP policies are currently configured?"

**🤖 AI Agent:**
> I found 1 IP policy: 'Office-Only-Access' (ID: ipp_789) which restricts access to the corporate CIDR range.


## Installation & Usage

To install and use the **ngrok** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ngrok](https://vinkius.com/mcp/ngrok)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
