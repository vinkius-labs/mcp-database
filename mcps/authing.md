# Authing MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/authing)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/authing-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/authing-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Cloud-native identity and access management platform — manage users, roles, and security logs via AI.

## Description
Empower your AI agent to orchestrate your entire identity infrastructure with **Authing**, the premier cloud-native IDaaS platform. By connecting Authing to your agent, you transform complex user management, organizational modeling, and security auditing into a natural conversation. Your agent can instantly list users, retrieve detailed profile metadata, browse organizational structures, and monitor security audit logs without you ever needing to navigate the comprehensive Authing console. Whether you are conducting a compliance audit or managing application access, your agent acts as a real-time identity assistant, keeping your user data accurate and your systems secure.

### What you can do

- **User Orchestration** — List and retrieve detailed information about users in your Authing user pool.
- **Organizational Management** — Browse and monitor organizational units and hierarchies across your company.
- **Access Control Auditing** — List roles, groups, and permission resources to identify authorization patterns.
- **Security Monitoring** — Retrieve real-time security audit logs to monitor administrative and user actions.
- **System Configuration** — Access high-level security settings and metadata for your identity projects.

### How it works

1. Subscribe to this server
2. Enter your Authing User Pool ID, Access Key, and Domain
3. Start managing your identity platform through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers** — automate compliance auditing and monitor system access through natural language queries.
- **IT Administrators** — manage user lifecycles and coordinate organizational changes directly from your AI-powered workspace.
- **Compliance Leads** — retrieve administrative logs and audit permission resources via a unified AI interface.
- **Authing Power Users** — integrate your existing identity workflows into your AI-driven daily routines to maintain peak operational efficiency.


## Available Tools
- **create_user**: Create a new user
- **get_audit_logs**: Get security audit logs
- **get_security_settings**: Get pool security settings
- **get_user**: Get user details
- **list_applications**: List registered applications
- **list_groups**: List user groups
- **list_organizations**: List organizations
- **list_resources**: List permission resources
- **list_roles**: List user roles
- **list_users**: List application users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Authing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all users in our Authing pool."

**🤖 AI Agent:**
> I've retrieved your Authing users. You have 150 registered members, including roles like 'Admin' and 'Developer'. Would you like to view the detailed profile for the last user created?

---

**👤 You:**
> "Show me the security audit logs from today."

**🤖 AI Agent:**
> I've listed today's audit logs. There are 12 administrative actions, including a role update for 'User8821' and 3 new application registrations. Should I retrieve more details for the sensitive actions?

---

**👤 You:**
> "List all organizational units in the company."

**🤖 AI Agent:**
> I've retrieved your organizational structure. You have 5 primary branches, including 'Engineering', 'HR', and 'Marketing'. Would you like to see the child units under 'Engineering'?


## Installation & Usage

To install and use the **Authing** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/authing](https://vinkius.com/mcp/authing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
