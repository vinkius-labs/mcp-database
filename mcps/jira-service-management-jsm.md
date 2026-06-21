# Jira Service Management (JSM) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jira-service-management-jsm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/jira-service-management-jsm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/jira-service-management-jsm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage service desks, customer requests, and queues via Jira JSM API.

## Description
Empower your AI agents with Jira Service Management's leading ITSM platform. This MCP server allows you to list service desks, retrieve customer requests, manage organizations and queues, and access knowledge base articles directly through the Jira JSM API. Ideal for automating IT support and service delivery workflows.


## Available Tools
- **get_info**: Use for system health monitoring.

Retrieves system information for the JSM instance
- **get_request**: g., "SD-123") or ID. Returns full descriptions, participants, and custom field values. Use this for deep investigation of a specific customer inquiry.

Retrieves details for a specific customer request
- **get_service_desk**: Returns project information and branding details. Useful for understanding the configuration of a specific support portal.

Retrieves details for a specific service desk
- **list_customers**: Useful for identifying support recipients and their account details.

Lists all customers for a specific service desk
- **list_knowledge_bases**: Essential for identifying available documentation that might help resolve common customer issues.

Lists all knowledge base articles for a specific service desk
- **list_organizations**: Useful for understanding which business entities are being supported and grouping support data by customer.

Lists all organizations in JSM
- **list_queues**: g., "All Open", "Unassigned") defined for a service desk. Useful for understanding how tickets are triaged and identifying backlog counts.

Lists all queues for a specific service desk
- **list_request_types**: g., "IT Help", "Hardware Request") available in a portal. Useful for understanding the service catalog of a specific team.

Lists all request types for a specific service desk
- **list_requests**: Includes request keys, summaries, and current status. Essential for monitoring the support queue and identifying urgent issues.

Lists all customer requests
- **list_service_desks**: Returns project keys, names, and IDs. Use this to identify the service desk ID before querying requests or queues.

Lists all service desks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jira Service Management (JSM)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active service desks in JSM."

**🤖 AI Agent:**
> I'll fetch the list of available service desks from your Jira Service Management instance.

---

**👤 You:**
> "Show me the latest customer requests."

**🤖 AI Agent:**
> I'll retrieve the most recent requests across all service desks for you.

---

**👤 You:**
> "Check the queues for service desk ID '1'."

**🤖 AI Agent:**
> I'll look up the current queues and their status for that specific service desk.


## Installation & Usage

To install and use the **Jira Service Management (JSM)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jira-service-management-jsm](https://vinkius.com/mcp/jira-service-management-jsm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
