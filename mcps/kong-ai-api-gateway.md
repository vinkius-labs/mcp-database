# Kong (AI API Gateway) MCP Server

Manage your API Gateway via Kong — orchestrate services, routes, and AI plugins directly from your agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kong-ai-api-gateway)

## Overview
**Category:** friends-mcp
**Tools Count:** 10

## Description
Connect your **Kong API Gateway** instance to any AI agent and take full control of your API lifecycle and AI traffic management through natural conversation.

### What you can do

- **Service Orchestration** — List backend services and create new upstream definitions defining URLs and protocols directly from your agent
- **Route Management** — Configure inbound routing rules to map client requests to backend services based on specific paths or hostnames
- **AI Plugin Control** — Apply and configure the `ai-proxy` plugin to enable LLM routing, model providers, and key encapsulation securely
- **Operational Patching** — Update existing plugin configurations in real-time, allowing you to adjust rate limits or swap AI models dynamically
- **Consumer CRM** — Manage consumer profiles and generate API keys for `key-auth` plugins to track specific user or tenant usage
- **Infrastructure Audit** — Discover enabled plugins across your gateway and remove unused modules instantly to maintain a clean proxy pipeline

### How it works

1. Subscribe to this server
2. Enter your Kong Admin URL and Admin Token
3. Start managing your API connectivity from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Platform Engineers** — manage global gateway configurations and audit enabled plugins through natural conversation
- **Backend Developers** — create new services and routes without leaving your terminal or switching to the Kong Manager UI
- **AI Ops Teams** — monitor and adjust AI Proxy settings to optimize LLM usage and provider costs across the organization


## Available Tools
- **list_consumers**: List all Consumer profiles registered in Kong
- **create_consumer_key**: Generate an API Key credential for a Kong Consumer
- **create_ai_plugin**: Frequently used for enabling the `ai-proxy` plugin for LLM routing and key encapsulation.

Apply a new Plugin (like AI Proxy) to a specific Service
- **create_route**: Create a new Route to expose a Service in Kong
- **create_service**: The payload must define the upstream URL, name, and protocol information.

Create a new backend Service in Kong
- **delete_plugin**: Delete and permanently remove a Plugin from the Kong Gateway
- **list_plugins**: g., Rate Limiting, AI Proxy, Key Auth) currently configured globally or scoped to specific Services/Routes.

List all enabled Plugins on the Kong Gateway
- **list_routes**: List all routing rules configured in the Kong API Gateway
- **list_services**: List all Services registered in the Kong API Gateway
- **update_plugin**: Useful for adjusting rate limits dynamically or swapping AI model providers under heavy load.

Update the configuration of an existing Kong Plugin


## Installation & Usage

To install and use the **Kong (AI API Gateway)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kong-ai-api-gateway](https://vinkius.com/mcp/kong-ai-api-gateway)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
