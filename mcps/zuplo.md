# Zuplo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zuplo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zuplo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zuplo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage API gateways, edge deployments, and consumers on Zuplo — the programmable API management platform for developers.

## Description
Connect your **Zuplo** account to any AI agent and manage your programmable API infrastructure through natural conversation.

### What you can do

- **Project Management** — List all Zuplo projects and API gateways in your account to monitor your integration landscape
- **Edge Deployments** — Trigger new configuration deployments to the global edge network or audit previous deployment history
- **Consumer Governance** — Create, manage, and revoke API key consumers to control who has access to your gateway authentication
- **Environment Auditing** — List available project environments (e.g., working, production) and verify their current operational status
- **DNS & Domains** — Retrieve and manage configured custom DNS domains for each of your API projects directly from your agent
- **Real-Time Metrics** — Monitor gateway traffic, latency, and throughput metrics directly from Zuplo's edge analytics network
- **Declarative Config** — Browse and list the configuration files that define your gateway's routing and policy logic

### How it works

1. Subscribe to this server
2. Enter your Zuplo API Key
3. Start managing your API gateways through Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex cloud consoles to whitelist a consumer. Your AI agent becomes your API platform engineer.

### Who is this for?

- **Platform Engineers** — monitor edge metrics and manage consumer identities through simple chat commands
- **API Developers** — trigger deployments and audit configuration files without manual data entry
- **DevOps Teams** — verify environment health and monitor custom domain configurations through conversation
- **Security Architects** — audit API key consumers and manage gateway authentication policies rapidly


## Available Tools
- **list_consumers**: List API key consumers
- **create_consumer**: Create API key consumer
- **create_deployment**: Create a new deployment
- **delete_consumer**: Delete API key consumer
- **list_custom_domains**: List custom domains
- **list_environments**: g., working, production) for a Project.

List project environments
- **list_files**: List configuration files
- **list_deployments**: List deployments
- **get_metrics**: Get edge metrics
- **list_projects**: List Zuplo projects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zuplo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Zuplo projects."

**🤖 AI Agent:**
> I found 3 Zuplo projects: 1. 'Payment-Gateway-Main' (ID: proj-101), 2. 'User-Auth-Edge' (ID: proj-102), and 3. 'Legacy-API-Proxy' (ID: proj-103). Which one would you like to see metrics for?

---

**👤 You:**
> "Check the latency metrics for 'proj-101'."

**🤖 AI Agent:**
> Latency metrics for proj-101: Average p95 latency is 42ms. Total traffic in the last 24h: 1.2 million requests. Current error rate: 0.05%. Everything looks healthy across the edge network.

---

**👤 You:**
> "Create a new consumer for 'Acme Partner' in project 'proj-101'."

**🤖 AI Agent:**
> Success! I've provisioned a new consumer identity for 'Acme Partner' (ID: cons-999) in project proj-101. I can provide the associated API key details if you need them for delivery.


## Installation & Usage

To install and use the **Zuplo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zuplo](https://vinkius.com/mcp/zuplo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
