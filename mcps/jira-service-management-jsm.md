# Jira Service Management (JSM) MCP Server

Manage service desks, customer requests, and queues via Jira JSM API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/jira-service-management-jsm)

## Overview
**Category:** industry-titans
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Jira Service Management (JSM)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jira-service-management-jsm](https://vinkius.com/mcp/jira-service-management-jsm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
