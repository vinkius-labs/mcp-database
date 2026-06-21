# Udesk / 沃丰科技 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/udesk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/udesk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/udesk-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Comprehensive customer service platform — manage tickets, customers, and knowledge base via AI.

## Description
Empower your AI agent to orchestrate your customer service operations with **Udesk**, the premier helpdesk platform in China. By connecting Udesk to your agent, you transform complex ticket management, customer profile auditing, and knowledge base retrieval into a natural conversation. Your agent can instantly list support tickets, retrieve detailed customer information, browse knowledge base articles, and even monitor agent activity without you ever needing to navigate the comprehensive web portal. Whether you are troubleshooting high-priority issues or coordinating support teams, your agent acts as a real-time service assistant, keeping your data accurate and your customers satisfied.

### What you can do

- **Ticket Orchestration** — List all support tickets and retrieve detailed subject and content metadata.
- **Customer Profile Control** — Browse helpdesk customers and retrieve detailed contact and organization information.
- **Agent Management** — List all support agents and identify functional groups within the service team.
- **Knowledge Retrieval** — Browse and retrieve articles from the internal knowledge base to accelerate resolution.
- **Activity Auditing** — Retrieve historical reply chains for tickets to monitor service quality.

### How it works

1. Subscribe to this server
2. Enter your Udesk Subdomain, Admin Email, and API Token
3. Start managing your customer service through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Managers** — monitor ticket progress and audit agent performance through natural language queries.
- **Customer Success Leads** — retrieve detailed customer profiles and interaction histories directly from your AI-powered workspace.
- **Service Operations** — oversee agent groups and coordinate cross-functional support via a unified AI interface.
- **Udesk Power Users** — integrate your existing service workflows into your AI-driven daily routines.


## Available Tools
- **create_ticket**: Create a new ticket
- **get_customer**: Get customer details
- **get_organization**: Get organization details
- **get_ticket**: Get ticket details
- **get_ticket_replies**: Get ticket reply history
- **list_agents**: List support agents
- **list_articles**: List knowledge base articles
- **list_customers**: List helpdesk customers
- **list_groups**: List agent groups
- **list_tickets**: List helpdesk tickets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Udesk / 沃丰科技** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active helpdesk tickets."

**🤖 AI Agent:**
> I've retrieved your Udesk tickets. You have 15 open incidents, including 'Server Down in Region A' and 'Billing Inquiry - Client B'. Would you like to check the latest replies for any of them?

---

**👤 You:**
> "Show me the details for customer 'mario@example.com'."

**🤖 AI Agent:**
> I've retrieved the profile for Mario. He is a VIP customer from the 'Global Partners' organization with 12 historical tickets. Would you like to see his active ticket history?

---

**👤 You:**
> "Check the knowledge base for articles about 'Refund Policy'."

**🤖 AI Agent:**
> I've found 3 articles in the Udesk knowledge base matching your query. The primary guide 'Standard Refund Procedures' was last updated 2 days ago. Should I retrieve the full content for you?


## Installation & Usage

To install and use the **Udesk / 沃丰科技** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/udesk](https://vinkius.com/mcp/udesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
