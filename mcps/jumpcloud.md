# JumpCloud MCP Server

Manage users, systems, and directories via JumpCloud API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/jumpcloud)

## Overview
**Category:** fort-knox
**Tools Count:** 10

## Description
Empower your AI agents with JumpCloud's open directory platform. This MCP server allows you to list and retrieve users, manage user and system groups, track managed systems, and view directories and SSO applications directly through the JumpCloud API. Ideal for automating IT administration and directory management.


## Available Tools
- **get_user**: Returns account metadata, group memberships, and security settings. Use this for detailed user vetting or before making administrative changes.

Retrieves details for a specific user
- **list_applications**: Useful for auditing software access and identifying which SaaS apps are integrated.

Lists all configured SSO applications
- **list_commands**: Useful for auditing automation scripts.

Lists saved management commands
- **list_directories**: Useful for auditing identity source configurations.

Lists all configured directories (LDAP, AD, Google, etc)
- **list_networks**: Useful for auditing WiFi and VPN authentication settings.

Lists all RADIUS networks
- **list_policies**: g., Disk Encryption, Firewall) defined in JumpCloud. Essential for auditing security compliance across the fleet.

Lists all system security policies
- **list_system_groups**: g., "Production Servers", "Employee Laptops"). Useful for identifying device cohorts for policy application.

Lists all system groups
- **list_systems**: Returns hostnames, IDs, and OS versions. Use this to audit company hardware and device compliance.

Lists all systems managed by JumpCloud
- **list_user_groups**: g., Marketing, Developers) configured in JumpCloud. Useful for understanding the organizational structure and access control policies.

Lists all user groups
- **list_users**: Returns usernames, IDs, and account status. Use this as the primary entry point for user auditing and identity management.

Lists all users in JumpCloud


## Installation & Usage

To install and use the **JumpCloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jumpcloud](https://vinkius.com/mcp/jumpcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
